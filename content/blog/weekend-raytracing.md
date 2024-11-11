+++
title = "Weekend Raytracing"
date = "2024-10-16T10:56:29+01:00"
tags = ["c", "graphics", "ray tracing", "learning"]
+++

Notes

- Red circle came out oblong due to dividing pixel delta by an int not float
- Creating solutions around the abstract base hittable and sphere concrete classes - just implement sphere for now as I don't need the expansion functionality of the base class, also c.
- First larger project using procedural code, used to using OOP with Python.
- First normal with ground had issues, ended up being lots of smaller bugs + wrongly setting main hit_rec value to temp value. Was doing hit_rec = &tmp_hit_rec. Should've been \*hit_rec = tmp_hit_rec. My guess, based off the images, is that the original hit_rec pointer was being set to a 'random' address associated with the temp value meaning it couldn't associate the different sphere objects.

This is a page about »Weekend Raytracing«.
