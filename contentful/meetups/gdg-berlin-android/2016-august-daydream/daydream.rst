:title: Daydreaming about Cardboards or Virtual Realtiy in Android
:charset: UTF-i8
:author: Mario Bodemann
:css: daydream.css
:skip-help: true
:data-transition-duration: 0

----

:data-x: 0
:data-y: 0
:data-z: 0
:data-rotate-y: 0


.. image:: images/cardboard.png
   :width: 200px

.. container:: scolling-background

  .. image:: images/scrolling-background.jpg
   :width: 20000px

.. container:: main-title

  Daydreaming about Cardboards

.. container:: main-subtitle

  Virtual Reality in Android

.. note::

        Do you want to ask the audience level? (``Android Pro/Medium/Beginner + VR Done'it/Knowsaboutit/new``)

----

:data-x: r1700


.. image:: images/contentful.png
   :width: 500px

* 🔧: headless CMS: `contentful.com <http://contentful.com/>`_
* 🐦: `@MarioBodemann <http://twitter.com/@MarioBodemann>`_
* 📄: `bit.ly/mbcbrd <http://bit.ly/mbcbrd>`_

.. note::

        * Please follow the slides at the given address.
        * Wait some seconds to see if someone is writing down the address...

----

.. image:: images/cardboard.png
   :class: center-image
   :width: 1000px 


----

Google Cardboard
----------------

* Easy to produce,
* available from different companies,
* in different styles/interactions,
* *You just need a phone.*

.. image:: images/cardboard-viewer.jpg
  :class: bottom-right 

----

How does Cardboard work?
------------------------

* Use 3D data and movement to draw two images,

  * one for the left and right eye.

* Contains Lenses to move things away.
* Brain combines image to 3D scene.

----

How do you program for it?
--------------------------

SDKs available for 

* Android (OpenGL),
* IOS (Objective C),
* Web (JS),
* Unity Engine (C# /JS) x (🍎, G,💻, 🐧).

----

How do I write a Unity App?
---------------------------

Demo time!
==========

.. image:: images/unity-editor-icon.png


.. note::
        
        * Clone googles github: https://github.com/googlevr/gvr-unity-sdk
        * Open Unity.
        * Add GameObject Plane(Rescale 10x10x10), Cube, Sphere, Cylinder, move/rotate(top gizmo) them around.
        * Download(?) a material from asset store, to assign to all models: Move Material to right hand object pool.
        * Assign rigid body (aka gravity) (Component/Physics/Rigid).
        * Duplicate some object to increase dynamic of scene. Play Scene.
        * Import the Unity package by going to Assets > Import Package > Custom Package.
        * Apply Camera by going to Assets/GoogleVR/Prefabs and move the GvrViewerMain onto the camera.
        * Play Scene. (Mention building it for Android and provide it later on)

        **Installing Unity on linux**

        * http://forum.unity3d.com/threads/unity-on-linux-release-notes-and-known-issues.350256/

----

What do those SDKs provide?
---------------------------

* Lens distortion correction.
* Spatial audio.
* Head tracking.
* 3D calibration.
* Side-by-side rendering.

----

What else do they provide?
--------------------------

* Stereo geometry configuration.
* User input event handling.
* See `developer.google.com/vr/android/ <https://developers.google.com/vr/android/>`_

----

What can I do in pure Android only?
-----------------------------------

* ``VrPanoramaView``/``VrVideoView``

  * Integration of photospheres in view hierarchies.

* Integration with other (Java) libraries.
* Sending of Intents easily.

----

Limitations of Android SDK
--------------------------

* Using 3D models has to be done by

  * either low level OpenGL or 
  * 3rd party 3d engine.

* Setup of ``Google VR`` libraries

  * one module for each ``.aar`` dependency needed.

----

Adding Photospheres to a simple project
---------------------------------------

* Demo
* How to add a Photosphere view to your view hierarchy.

.. image:: images/nougat_2x.png
   :class: bottom-right

.. note::

        * Open Android Studio.
        * Open ``Simple Android List View`` project.
        * Show current status in ``Vysor``.
        * Add three dependencies by hand: ``Common, CommonWidget, PanoWidget (Sources/Others/gvr-android-sdk/libraries)``
        * Use VrPanoramaView in xml, increasing the ``height`` of view.
        * Use VrPanoramaView in java (adapter)
        * Load image from resources. (``VrPanoramaView.load``, ``BitmapFactory.decoderesource)``

----

:data-x: 0
:data-y: 1000

.. image:: images/daydream-logo.png
   :class: center-image
   :width: 1000px

.. note::

        * Introduced at Google I/O this year.
        * Soon™ first hardware available.

----

:class: hide-background
:data-x: r1700

.. image:: images/daydream-headset.png
   :height: 800px

Google IO 2016 `General <https://youtu.be/rOCaujUOCuE>`_ `Controller <https://www.youtube.com/watch?v=l9OfmWnqR0M>`_ `Designing <https://www.youtube.com/watch?v=00vzW2-PvvE>`_


----

:class: hide-background
:data-x: r190
:data-y: r240
:data-z: r-800

.. note::

        Controller

        * Uses special hardware as controller.

                * Can get emulated by any Android phone (>= 4.4).
                * Has four Buttons: Volume +/-, App(Programmable), Home.
                * Clickable Touchpad. (x/y position, clicked state)(Emulated by two touches)

        * Print out sheet to not get to disctracted by Phone
        * Connects via bluetooth to ``Headset Phone``.

----

:class: hide-background
:data-x: r-400
:data-y: r-12
:data-z: r100

.. note::

        Headset Phone

        * Has to be a ``Nexus 6p`` running ``Android Nougat 7.0``.
        * Start a Daydream app once, set it up by clicking on the ``Gear``, enabling all VR settings.
        * ``Reboot phone ...`` ;) .
        * Bluetooth to connect to Controller.

----

:class: hide-background
:data-x: r210
:data-y: r-228
:data-z: r700


.. note::

        Complete Package

        * ``Daydream Ready``

                * High performance sensors for high accuracy head tracking.
                * Displays with fast response time to minimize blur.
                * Powerfull mobile processor.
                * VR System notifications.

        * Will be available ``in fall``.
        * Will be created by hardware partners.
        * Certified by ``Google``.
        * Google Play for VR and ``Daydream Home``

----

:data-x: r1700
:data-y: r0
:data-z: r0

New SDK features
----------------

* Controlling the controller

  * Orientation/Acceleration 
  * Clickpad
  * Buttons

* Spatial Audio Engine

----

Deprecation & Deletion
----------------------

* ``Deprecation of v1 Cardboards`` 😱
* Deprecation of Cardboard Button infavor of Controller
* Renaming ``Cardboard*`` to ``Gvr*``

----

:data-x: -1700
:data-y: 1900
:data-z: 2000
:data-rotate-x: 0
:data-rotate-y: -60
:data-rotate-z: 90
:class: last-slide

Thank you
=========

