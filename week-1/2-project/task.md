# Readwell

Your friend Kayla needs your help!

A few months ago, Kayla built a simple website called “Readwell”. On Readwell, you can discover classic books to read online.

Soon, Kayla’s website became very popular! However, some users were getting angry, because it was too slow. This is because Kayla was putting all her data into multiple files, and she soon got too many files.

Then, Kayla decided to use MongoDB. She heard that it was better for lots of data. She spent a long time turning her files into documents on a MongoDB server.

However, Kayla does not know how to connect her server to the MongoDB database! Luckily, she knows someone who can do it: you!

Your job is to rewrite her Express server endpoints to correctly get books from her database collection.

## Endpoints

You need to write two endpoints:
```
/api/books
/api/books/:id
```

1. When you go to `/api/books`, you should get all books.

2. If you add the query parameter title or author, you should get only books with the title or author value.

3. If you add both of those query parameters, you should only get books with both the title and the author value.

   - For example, `/api/books?author=Jane Austen&title=Pride` and Prejudice should only get books with the author Jane Austen and title Pride and Prejudice.

4. When you go to `/api/books/:id`, you should only get the book with that ID.

   - For example, if you go to `/api/books/5cfc28b7af37addd3cb1e7d2`, you should only get the book with `"\_id": "5cfc28b7af37addd3cb1e7d2"`.

5. If you give an ID that you cannot use for an ObjectId, you should get a 400 response.

6. If you give a valid ObjectId string but it has no book, you should get a 404 response.

## Details

Start by remixing this code:

https://glitch.com/~cyf-db-lesson-1-homework

Here is the database URI:

`mongodb+srv://cyf:LetsLearnMongoDB2019@cluster0-cxacx.mongodb.net`

The database is literature, and the collections is books.
