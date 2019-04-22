Return ALL the data in the 'movies' table.
SELECT * FROM movies;

Return ONLY the name column from the 'people' table
SELECT name FROM people;

Oops! Someone at CodeClan spelled Rose's name wrong! Change it to reflect the proper spelling ('Rose' not 'Ros').
UPDATE people
SET name = 'Rose Ulldemolins'
WHERE name = 'Ros Ulldemolins';

Return ONLY your name from the 'people' table.
SELECT name FROM people
WHERE name = 'Rose Ulldemolins';

The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.
DELETE FROM movies
WHERE title = 'Batman Begins';

Create a new entry in the 'people' table with the name of one of the instructors.
INSERT INTO people (name) VALUES ('Keith Douglas');

Donald Trump has decided to hijack our movie evening, Remove him from the table of people.
DELETE FROM people
WHERE name = 'Donald Trump';

The cinema has just heard that they will be holding an exclusive midnight showing of 'Avengers: Infinity War'!! Create a new entry in the 'movies' table to reflect this.
INSERT INTO movies (title, year, show_time) VALUES ('Avengers: Infinity War', '2019', '00:00');

The cinema would also like to make the Guardians movies a back to back feature. Find out the show time of "Guardians of the Galaxy" and set the show time of "Guardians of the Galaxy 2" to start two hours later.
SELECT show_time FROM movies
WHERE title = 'Guardians of the Galaxy';
UPDATE movies
SET show_time = '16:25'
WHERE title = 'Guardians of the Galaxy';
