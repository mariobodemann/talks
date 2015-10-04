:title: Android Study Jam, Lesson 6: Services and Notifications
:author: Mario Bodemann
:css: lesson.css

----

:data-x: 0
:data-y: 0
:data-z: 0
:data-rotate-y: 0

.. container:: main-title

  Android Beginners recap - lesson 1

.. image:: images/octobear.png
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

← Drinks/Toilet
===============

----

:data-x: -400
:data-y: r200
:data-z: -1400
:data-rotate-y: 216

WiFi password →
===============

----

:data-x: -800
:data-y: r200
:data-z: -1000
:data-rotate-y: 288

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

:data-x: r0
:data-y: r0
:data-z: 3000
:data-rotate-x: 30
:data-rotate-y: 75
:data-rotate-z: 30
:class: new-section

**Done. YOU ARE GREAT**
=======================

Now celebrate, what was your own project about?
-----------------------------------------------

