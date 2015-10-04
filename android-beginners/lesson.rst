:title: Android Development for Beginners - lesson 1
:author: Mario Bodemann
:css: lesson.css

----

:data-x: 0
:data-y: 0
:data-z: 0

.. container:: main-title

  Android Development for Beginners

.. container:: main-subtitle

  Lesson 1: the begining

.. image:: images/octobear2x.png
   :height: 700

----

:data-x: 40
:data-y: 100
:data-z: 50
:data-scale: .15
:data-rotate-x: -35

Thanks to 
=========

.. image:: images/thoughtworks-logo.png


for this space
--------------

and Udacity_ 
============

for the lessons
---------------

.. _Udacity: https://www.udacity.com/course/android-development-for-beginners--ud837

----

:class: new-section

:data-x: 279
:data-y: 0
:data-z: 25
:data-scale: .02
:data-rotate-x: 0


What? How?
==========

What will this course be about and how do we organize it?
---------------------------------------------------------

----

:data-x: r40
:data-y: 0

← Drinks/Toilet
===============

----


WiFi password →
===============

----


Hi, my name is *Mario*, and who are *you*?
==========================================

----

:class: code-slide

*SunshineService.java* (merged with *FetchWeatherTask*)

.. code:: java

  public class SunshineService extends IntentService {
    public SunshineService() {
        super("SunshineService");
    }

     @Override
    protected void onHandleIntent(Intent intent) {
        if (intent != null && 
            intent.hasExtra(LOCATION_EXTRA)) {
            doInBackground(
                intent.getStringExtra(LOCATION_EXTRA));
        }
    }

    protected void doInBackground(String location) {
        if (TextUtils.isEmpty(location)) {
            return;
        }
   }
 } 

----

:class: new-section

**Done. YOU ARE GREAT**
=======================

Now celebrate, what was your own project about?
-----------------------------------------------

