# -
ДЗ нетология Mongo db

1/ 
db.books.insertMany([
  {
    title: "Book One",
    description: "Description of Book One",
    authors: "Author One"
  },
  {
    title: "Book Two",
    description: "Description of Book Two",
    authors: "Author Two"
  }
]);

2/// 
db.books.find({ title: "Book One" });

3///
db.books.updateOne(
  { _id: ObjectId("id") },
  {
    $set: {
      description: "Updated description",
      authors: "Updated author"
    }
  }
);
