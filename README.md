# CS-3980-Assignment-3

db.movies.find(
  { year: 1983, runtime: { $gt: 200 } },
  { runtime: 1, title: 1, year: 1, _id: 0 }
).sort({ runtime: 1 })


![Plot](screenshot_1.png)


db.movies.find(
  { year: { $gt: 2014 }, "imdb.rating": { $gt: 9 } },
  { title: 1, year: 1, "imdb.rating": 1, _id: 0 }
).sort({ title: 1 })

![Plot](screenshot_2.png)

