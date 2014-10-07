---
title: Fake Wrong Gilt Notes
---

Introduction
============

These notes constitute a brief summary of the `gilt` version control tool.
They are incorrect, and it is your task to find and correct the mistakes.

You are judged, however, not on finding all the mistakes, but on your use of version control
in doing the work of fixing them!

Finding the mistakes will be a useful revision, though.

Activating Gilt
==============

To turn on the version control system, use:

``` bash
cd my_work_folder
gilt begin
```

Tell Gilt about a new file
======================

```
vim my_file # Edit file
gilt include my_file
```

Include changes in a file into the next work chunk 
==============================================

```
gilt include my_file
```

This includes the changes to that file in a list of changes
currently scheduled to be included in the next work chunk.

Include all scheduled changes into a work chunk
===============================================

```
gilt chunk -m "Journal entry"
```

Store all scheduled changes in a new chunk
==========================================

```
gilt include --uptodate
```

Include all changes *and* chunk them
====================================

```
gilt chunk -am "Journal entry"
```

View list of recent chunks
==========================

```
gilt journal
```

Transmit chunks to remote chunkstore
====================================

```
gilt transmit
```

Fetch chunks from remote chunkstore
===================================

```
gilt download
```
