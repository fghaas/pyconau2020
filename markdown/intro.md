## What I now know about HAproxied Django DB connections
... and wish I'd known sooner

* * *

Florian Haas [@xahteiwi](https://twitter.com/xahteiwi) ![City Network logo](images/citynetwork-logo.svg) <!-- .element class="inline" --> [City Network](https://www.citynetwork.eu/)

PyCon AU 2020

2020-09-04

<!-- Note -->
Hello dear PyCon AU people, I’m here to talk about an issue that my
team and I ran into a few months ago, which has to do with the very
interesting behavior of asynchronous Celery tasks that talk to a MySQL
or MariaDB cluster via HAProxy.

Hence the title, “what I now know about HAproxied Django database
connections, and wish I’d known sooner.”

Let’s start with some basics to set the stage.
