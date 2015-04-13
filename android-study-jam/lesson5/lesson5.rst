:title: Android Study Jam, Lesson 5
:author: Mario Bodemann
:css: lesson5.css

----

:data-x: 0
:data-y: 0
:data-z: 0
:data-rotate-y: 0

.. container:: main-title

  Android Study Jam: Lesson 5

.. container:: main-subtitle

  Rich and Responsive Layouts

.. image:: images/android_robot_200.png
   :height: 700

----

:data-x: 800
:data-y: r200
:data-z: -1000
:data-rotate-y: 72

Thanks to 
=========

.. image:: images/thoughtworks-logo.png

for this space
==============

----

:data-x: 400
:data-y: r200
:data-z: -1400
:data-rotate-y: 144

<-- Drinks/Toilet
=================

----

:data-x: -400
:data-y: r200
:data-z: -1400
:data-rotate-y: 216

WiFi password -->
=================

----

:data-x: -800
:data-y: r200
:data-z: -1000
:data-rotate-y: 288

Hi, my name is *Mario*, and who are *you*?
==========================================

----

:data-rotate-y: 359
:data-x: 0
:data-y: 1200
:data-z: 0
:class: new-section

Lesson 4
========

Database, Content Provider, Resolver and Loader
-----------------------------------------------

----

:data-x: r1400
:data-y: r0
:data-z: r0
:data-rotate-y: 360

Summary
=======

.. image:: images/lesson4-summary.png
   :width: 1000px

----

Sqlite
======

.. image:: images/lesson4-databases.jpg  

----

Provider
========

.. image:: images/lesson4-content-provider-step-0.png  

----

.. image:: images/lesson4-content-provider-step-2.png  

----

.. image:: images/lesson4-content-provider-step-1.png  

----

.. image:: images/lesson4-content-provider-step-3.png  

----

Loader
======

.. image:: images/lesson4-loader.png

----

:data-rotate-y: 0
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

