:title: Android Study Jam, Lesson 5
:author: Mario Bodemann
:css: lesson5.css

----

:data-rotate-y: -60

.. container:: main-title

  Android Study Jam: Lesson 5

.. container:: main-subtitle

  Content Loader

.. image:: images/android_robot_200.png
   :height: 700

----

:data-x: r1600
:data-rotate-y: 0

Thanks to 
=========

.. image:: images/thoughtworks-logo.png

for this space
==============

----

<-- Drinks/Toilet
=================

----

WiFi password -->
=================

----

Hi, my name is *Mario*, and who are *you*?
==========================================

----

:class: new-section

Lesson 4
========

Database, Content Provider, Resolver and Loader
-----------------------------------------------

----

:class: new-section

Lesson 5
========

Rich and Responsive Layouts
---------------------------

----

:class: code-slide

.. code:: java
    
    public class ForecastFragment 
        extends Fragment 
        implements LoaderManager.LoaderCallbacks<Cursor> {

    private static final int LOADER_WEATHER_ID = 0;

    // [...]

    @Override
    public void onActivityCreated(@Nullable Bundle 
        savedInstanceState) {
     
        super.onActivityCreated(savedInstanceState);
        getActivity().getLoaderManager().initLoader(
            LOADER_WEATHER_ID, null, this);
    }
    }

----

:data-x: r1200
:data-y: r-1000
:data-z: 1500
:data-rotate-y: -75
:data-rotate-x: 0

Done.
=====

Questions???
------------

