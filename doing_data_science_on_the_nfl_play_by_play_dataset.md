### Doing Data Science on the NFL Play By Play Dataset

Jesse Anderson - Curriculum Developer and Instructor - Cloudera

Advanced NFL stats released all Play By Play since 2002 season 471,000+ plays

[jesse-anderson.com](http://jesse-anderson.com) has chart of some of this data

his custom map-reduce code is up on his github account

Middle portion of every nfl record was in unstructured data.  Just a sentence of what happened, ex: 
>(2:48) C.Kaepernick pass short right to M.Crabtree to SD 25 for 1 yard (C.Tillman). Caught at SF 25. 0-yds YAC

Sentiment analysis, the ability to determine whether people are content or upset based on the content of the text.

[Hive](https://hive.apache.org/) provides an abstraction on top of MapReduce.  Allows queries using a SQL-like language to query unstructured data.

@jessetanderson

[github.com/eljefe6a/nfldata](http://github.com/eljefe6a/nfldata) code on this data