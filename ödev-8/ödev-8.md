## SQL ÖDEV - 8

1. Test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

    ```SQL
    CREATE TABLE employee (
    id SERIAL PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    birthday DATE,
    email VARCHAR(100)
    );
    ```

2. Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

    ```SQL
    insert into employee (name, email, birthday) values ('Dorey McCool', 'dmccool0@yale.edu', '1902-10-05');
    insert into employee (name, email, birthday) values ('Barth De Cleyne', 'bde1@shop-pro.jp', '2019-07-14');
    insert into employee (name, email, birthday) values ('Charil Amys', 'camys2@privacy.gov.au', '1965-12-27');
    insert into employee (name, email, birthday) values ('Eveleen Triggol', 'etriggol3@biglobe.ne.jp', '2013-01-08');
    insert into employee (name, email, birthday) values ('Josefina Hedge', 'jhedge4@independent.co.uk', '1901-11-15');
    insert into employee (name, email, birthday) values ('Kordula Eliot', 'keliot5@senate.gov', '1990-11-20');
    insert into employee (name, email, birthday) values ('Benoite Chaudrelle', 'bchaudrelle6@bbb.org', '1916-08-15');
    insert into employee (name, email, birthday) values ('Hyacinth Jeanenet', 'hjeanenet7@squarespace.com', '1942-01-11');
    insert into employee (name, email, birthday) values ('Baxy Cammish', 'bcammish8@unicef.org', '1914-12-05');
    insert into employee (name, email, birthday) values ('Nichole Babidge', 'nbabidge9@nature.com', '2018-10-13');
    insert into employee (name, email, birthday) values ('Jena Clilverd', 'jclilverda@nationalgeographic.com', '1989-07-31');
    insert into employee (name, email, birthday) values ('Anabel Southern', 'asouthernb@squidoo.com', '1936-05-09');
    insert into employee (name, email, birthday) values ('Wood Gamblin', 'wgamblinc@theatlantic.com', '2004-10-04');
    insert into employee (name, email, birthday) values ('Craggie Whenman', 'cwhenmand@people.com.cn', '1973-08-24');
    insert into employee (name, email, birthday) values ('Kala Bagot', 'kbagote@un.org', '2015-01-29');
    insert into employee (name, email, birthday) values ('Melissa Cussons', null, null);
    insert into employee (name, email, birthday) values ('Paulita Mews', 'pmewsg@deliciousdays.com', '2011-07-10');
    insert into employee (name, email, birthday) values ('Leisha Clausson', 'lclaussonh@yelp.com', '1959-07-19');
    insert into employee (name, email, birthday) values ('Emilie Jackett', 'ejacketti@virginia.edu', '1940-03-27');
    insert into employee (name, email, birthday) values ('Annelise Pain', 'apainj@cnn.com', '1979-08-07');
    insert into employee (name, email, birthday) values ('Gaven Kleinholz', 'gkleinholzk@e-recht24.de', '2004-12-29');
    insert into employee (name, email, birthday) values ('Quentin Abbotson', 'qabbotsonl@netlog.com', '1999-08-30');
    insert into employee (name, email, birthday) values ('Mack Douberday', 'mdouberdaym@drupal.org', '1935-04-11');
    insert into employee (name, email, birthday) values ('Debora Brunker', 'dbrunkern@sakura.ne.jp', '2007-08-04');
    insert into employee (name, email, birthday) values ('Rooney Mulkerrins', 'rmulkerrinso@yelp.com', '1967-11-20');
    insert into employee (name, email, birthday) values ('Killy Devany', 'kdevanyp@ucoz.ru', '1974-01-01');
    insert into employee (name, email, birthday) values ('Freddie Crohan', 'fcrohanq@adobe.com', '1987-06-11');
    insert into employee (name, email, birthday) values ('Rebe Riepel', 'rriepelr@vinaora.com', '2003-08-30');
    insert into employee (name, email, birthday) values ('Erek Mourant', 'emourants@joomla.org', '1992-10-31');
    insert into employee (name, email, birthday) values ('Rosalind Loyndon', 'rloyndont@nps.gov', '1982-06-16');
    insert into employee (name, email, birthday) values ('Ashleigh Brader', 'abraderu@illinois.edu', '1940-05-07');
    insert into employee (name, email, birthday) values ('Gertrudis Trustey', 'gtrusteyv@xrea.com', '1948-10-05');
    insert into employee (name, email, birthday) values ('Ari Leary', 'alearyw@nature.com', '1972-12-12');
    insert into employee (name, email, birthday) values ('Jaine Casotti', 'jcasottix@yahoo.com', '1978-10-11');
    insert into employee (name, email, birthday) values ('Valle Boyes', 'vboyesy@angelfire.com', '1972-10-27');
    insert into employee (name, email, birthday) values ('Read Vedyashkin', 'rvedyashkinz@aboutads.info', '1932-10-02');
    insert into employee (name, email, birthday) values ('Abie Illem', 'aillem10@squidoo.com', '2016-01-03');
    insert into employee (name, email, birthday) values ('Sky Glidden', 'sglidden11@topsy.com', '1965-11-28');
    insert into employee (name, email, birthday) values ('Aylmar Bathurst', 'abathurst12@feedburner.com', '2013-01-05');
    insert into employee (name, email, birthday) values ('Patty La Padula', 'pla13@alexa.com', '1992-08-20');
    insert into employee (name, email, birthday) values ('Ambros Mee', 'amee14@japanpost.jp', '1939-12-13');
    insert into employee (name, email, birthday) values ('Vanya Henworth', 'vhenworth15@clickbank.net', '1913-04-30');
    insert into employee (name, email, birthday) values ('Aurelie Livings', 'alivings16@un.org', '2010-05-26');
    insert into employee (name, email, birthday) values ('Adam Cliburn', 'acliburn17@google.com', '1955-10-01');
    insert into employee (name, email, birthday) values ('Mariska Slowey', 'mslowey18@chronoengine.com', '1998-11-23');
    insert into employee (name, email, birthday) values ('Cherish Sharratt', 'csharratt19@forbes.com', '1967-11-05');
    insert into employee (name, email, birthday) values ('Michal Stinchcombe', 'mstinchcombe1a@elegantthemes.com', '1954-12-14');
    insert into employee (name, email, birthday) values ('Vanna Haines', 'vhaines1b@w3.org', '1983-09-14');
    insert into employee (name, email, birthday) values ('Malena Ebben', null, null);
    insert into employee (name, email, birthday) values ('Kearney Quinby', 'kquinby1d@jiathis.com', '1941-07-21');
    ```

3. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

    ```SQL
    UPDATE employee
    SET name = 'Updated name'
    WHERE id = 22
    RETURNING *;

    UPDATE employee
    SET name = 'Updated date'
    WHERE name LIKE 'D%'
    RETURNING *;

    UPDATE employee
    SET birthday = '2022-06-30'
    WHERE birthday = '1950-01-01'
    RETURNING *;

    UPDATE employee
    SET email = 'updated@email.com'
    WHERE id > 48
    RETURNING *;

    UPDATE employee
    SET name  = 'XXXX - YYYY'
    WHERE birthday = '2000-01-01'
    RETURNING *;
    ```

4. Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

    ```SQL
    DELETE FROM employee
    WHERE id = 22
    RETURNING *;

    DELETE FROM employee
    WHERE name LIKE 'D%'
    RETURNING *;

    DELETE FROM employee
    WHERE birthday = '1950-01-01'
    RETURNING *;

    DELETE FROM employee
    WHERE id > 48
    RETURNING *;

    DELETE FROM employee
    WHERE birthday = '2000-01-01'
    RETURNING *;
    ```
