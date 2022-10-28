# Introduction

```{tableofcontents}
```

<hr>

The American Heart Association (AHA) collects an abundance of patient data from many different hospitals internationally. For example, the [Get With The Guidelines (GWTG)](https://www.heart.org/en/professional/quality-improvement) registry data alone comes from over 2,400 hospitals across the United States alone with more than 9 million total patient records entered and collated for medical researchers to use. 

As such, it is important that his data is securely stored in a way where both its management and distribution can remain simplified despite the amount of data scaling up. This is where the database comes into play.

The AHA Registry Database is a collection of organized data from different registries, powered by the [Django framework](https://www.djangoproject.com/) and coded in Python. The registry database has two main goals:
- Improving the efficiency, accuracy, and security of the whole management process for all AHA registry data.
- Building a user-friendly portal to promote and facilitate the data access control, exploration, and research for both AHA data administrators and researchers within and outside of AHA. 

Given the complex nature of navigating through the Django framework and understanding custom features, **the purpose of this document is to provide internal developers (i.e. AHA Staff) with a reference manual for anything related to the development of this database, both the backend development and the frontend Django user interface**. 