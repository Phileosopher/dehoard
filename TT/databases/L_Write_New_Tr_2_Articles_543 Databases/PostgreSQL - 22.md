
[PostgreSQL 16 | Hacker News](https://news.ycombinator.com/item?id=37508471)
[PostgreSQL: PostgreSQL 16 Released!](https://www.postgresql.org/about/news/postgresql-16-released-2715/)

[PostgreSQL reconsiders its process-based model | Hacker News](https://news.ycombinator.com/item?id=36393030)
[PostgreSQL reconsiders its process-based model [LWN.net]](https://lwn.net/Articles/934940/)

[Postgres is a great pub/sub and job server (2019) | Hacker News](https://news.ycombinator.com/item?id=29599132)
[Postgres is a great pub/sub & job server](https://webapp.io/blog/postgres-is-the-answer/)

[An unexpected find that freed 20GB of unused index space in PostgreSQL | Hacker News](https://news.ycombinator.com/item?id=25988871)
[An unexpected find that freed 20GB of unused index space (2021) | Hacker News](https://news.ycombinator.com/item?id=37294793)
[The Unexpected Find That Freed 20GB of Unused Index Space | Haki Benita](https://hakibenita.com/postgresql-unused-index-size)

[PostgreSQL community impact of 2nd Quadrant purchase | Hacker News](https://news.ycombinator.com/item?id=24710759)
[Bruce Momjian: Postgres Blog](https://momjian.us/main/blogs/pgblog/2020.html#October_7_2020)

[FOSDEM 2019 - PostgreSQL vs. fsync](https://archive.fosdem.org/2019/schedule/event/postgresql_fsync)

[Things I hate about PostgreSQL (2020) | Hacker News](https://news.ycombinator.com/item?id=26709019)
[10 Things I Hate About PostgreSQL | by Rick Branson | Medium](https://rbranson.medium.com/10-things-i-hate-about-postgresql-20dbab8c2791)

[Just use Postgres for everything | Hacker News](https://news.ycombinator.com/item?id=33934139)
[Just Use Postgres for Everything | Amazing CTO](https://www.amazingcto.com/postgres-for-everything/)

[SQL Maxis: Why We Ditched RabbitMQ and Replaced It with a Postgres Queue | Hacker News](https://news.ycombinator.com/item?id=35526846)
[SQL Maxis: Why We Ditched RabbitMQ And Replaced It With A Postgres Queue](https://www.prequel.co/blog/sql-maxis-why-we-ditched-rabbitmq-and-replaced-it-with-a-postgres-queue)

[Choose Postgres queue technology | Hacker News](https://news.ycombinator.com/item?id=37636841)
[Choose Postgres queue technology :: Adriano Caloiaro's personal blog](https://adriano.fyi/posts/2023-09-24-choose-postgres-queue-technology/)

[Postgres: The next generation | Hacker News](https://news.ycombinator.com/item?id=37832319)
[Postgres: the next generation. Investing in the next generation of committers. - James Governor's Monkchips](https://redmonk.com/jgovernor/2023/10/10/postgres-the-next-generation-investing-in-the-next-generation-of-committers/)

[PostgreSQL is enough | Hacker News](https://news.ycombinator.com/item?id=39273954)
[Postgres is Enough](https://gist.github.com/cpursley/c8fb81fe8a7e5df038158bdfe0f06dbb)

[Postgres as queue | Hacker News](https://news.ycombinator.com/item?id=39315833)
[leontrolski - postgres as queue](https://leontrolski.github.io/postgres-as-queue.html)

[My notes on Gitlab's Postgres schema design (2022) | Hacker News](https://news.ycombinator.com/item?id=39413972)
[My Notes on GitLab Postgres Schema Design - Shekhar Gulati](https://shekhargulati.com/2022/07/08/my-notes-on-gitlabs-postgres-schema-design/)

[I wrote a new JIT compiler for PostgreSQL | Hacker News](https://news.ycombinator.com/item?id=39742916)
[Look ma, I wrote a new JIT compiler for PostgreSQL - Pinaraf's website](https://www.pinaraf.info/2024/03/look-ma-i-wrote-a-new-jit-compiler-for-postgresql/)

[Simon Riggs has died | Hacker News](https://news.ycombinator.com/item?id=39861680)
[Berkubernetus: "PostgreSQL maintainer Simon Riggs has died in a s…" - M6n.io](https://m6n.io/@fuzzychef/112172393647826741)

[Show HN: I open-sourced the in-memory PostgreSQL I built at work for E2E tests | Hacker News](https://news.ycombinator.com/item?id=39960537)
[stackframe-projects/pgmock: In-memory Postgres for unit/E2E tests](https://github.com/stackframe-projects/pgmock)

[Ten years of improvements in PostgreSQL's optimizer | Hacker News](https://news.ycombinator.com/item?id=40060123)
[Ten years of improvements in PostgreSQL's optimizer · Ryan Marcus](https://rmarcus.info/blog/2024/04/12/pg-over-time.html)

[PostgreSQL and UUID as Primary Key | Hacker News](https://news.ycombinator.com/item?id=40884878)
[Maciej Walkowiak | PostgreSQL and UUID as primary key](https://maciejwalkowiak.com/blog/postgres-uuid-primary-key/)

[Dzmitry Plashchynski](https://medium.com/@plashchynski/postgresql-upgrade-on-centos-4c0ddd2f8687)
(2016) PostgreSQL upgrade on CentOS
applicable to all Red Hat family (RHEL/CentOS/SL/OL 7) and to all PostgreSQL 9.* versions.

[Stack Overflow](https://stackoverflow.com/questions/876522/creating-a-copy-of-a-database-in-postgresql)
Creating a copy of a database in PostgreSQL.
in essence, what works for me :
```
# backup :
pg_dumpall > db.out
# restore :
# (might requires some DROP DATABASE xxx if you do want to replace existing data with same db and table names)
psql -f db.out postgres
```

[Creating a search engine with PostgreSQL | Hacker News](https://news.ycombinator.com/item?id=36699016)
[Create an advanced search engine with PostgreSQL](https://xata.io/blog/postgres-full-text-search-engine)
