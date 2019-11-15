# Grading Assets

When looking to promote the reuse of shared services and components it must be realised that not every asset is intended or suitable for reuse.  

* Some assets are appropriate only for the application for which they are created.
* Some assets are appropriate for reuse within a department but have little or no relevance or purpose outside of that department.
* Some assets are appropriate for reuse right across departments and potentially could be shared NICS wide.

There needs to be standards for grading assets and a repeatable method for doing so.   This document lays out those standards.

## Enterprise Grade
If an asset is intending to deliver some or all of a shared capability identified in an [architecture blueprint.  Link is tbd](http://link-tbd), or implement master data management for a key domain data type/entity, then it is a candidate for being an Enterprise grade asset.

## Department Grade
If an asset handles domain events or entities that are relevant across an entire department - but not outside of that department - then the asset is a candidate for being a Department grade asset.  

For example there may be applications supporting processes around school inspections that are only relevent to the Department of Education.  That asset is likely useful and reusable across that department but may well not be relevant outside of DoE.

## Application Grade
If an application is created to implement specific business value to one team/branch then and isn't deemed to be an enterprise grade or department grade asset then it is considered to be an application grade asset.


### Personal thoughts / objections
I introduce the idea of something being a candidate for being an enterprise grade or department grade. Should I just drop that?  Should there not be a way of putting forward an asset as a candidate to be considered - and accepted or rejected - by architecture?


