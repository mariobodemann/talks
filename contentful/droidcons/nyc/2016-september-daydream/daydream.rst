:title: Daydreaming about Cardboards or Virtual Realtiy in Android
:charset: UTF-8
:author: Mario Bodemann
:css: daydream.css
:skip-help: true
:data-transition-duration: 0

----

:class: hide-background

.. container:: scolling-background

  .. image:: images/scrolling-background-blocky.png
   :width: 30000px

.. container:: main-title

  Daydreaming about Cardboards

.. container:: main-subtitle

  Virtual Reality in Android

----

:data-x: r2000

.. image:: images/contentful.png
   :width: 500px

* 🔧: headless CMS: `contentful.com <http://contentful.com/>`_
* 🐦: `@MarioBodemann <http://twitter.com/@MarioBodemann>`_
* 📄: `bit.ly/mbvrberlin <http://bit.ly/mbvrvienna>`_

  * Please interrupt `👄👅 <http://blah.de/>`_!

.. note::
   * Please follow the slides at the given address.
   * Wait some seconds to see if someone is writing down the address...
   
   Audience
   
   * ``Android programmer? 👋``
   * ``VR programmer? 👋``

----

:data-x: -1000
:data-y: 2300
:data-z: 0
:data-scale: 6
:class: hide-background

Agenda

----

:data-x: 0
:data-y: 1300
:data-z: 0
:data-rotate-x: 0
:data-rotate-y: 0
:data-rotate-z: 0
:data-scale: 1

.. image:: images/cardboard.png
   :class: center-image
   :width: 1000px 

----

:data-x: r2000
:data-y: r0

Google Cardboard
----------------

* easy to produce
* available from different companies
* in different styles/interactions
* *You just need a phone™*

.. image:: images/cardboard-viewer.jpg
  :class: bottom-right 

----

How does Cardboard work?
------------------------

* use 3D data and movement to draw two images

  * one for the left and right eye

* contains Lenses to move things away
* brain combines image to 3D scene

----

.. image:: images/contentful-vr-bunny.gif
   :class: center-image

----

How do you program for it?
--------------------------

Googles SDK are available for

* Android (OpenGL)
* iOS (Objective C)
* Unreal Engine (*NEW*)
* Unity Engine (C# /JS) x (🍎, G,💻, 🐧)

----

What do those SDKs provide?
---------------------------

* lens distortion correction
* spatial audio
* head tracking
* 3D calibration
* side-by-side rendering

----

What else do they provide?
--------------------------

* stereo geometry configuration
* user input event handling
* see `https://vr.google.com/developers/ <https://vr.google.com/developers/>`_

----

:data-x: 0
:data-y: r1300

How do I write a Unity App?

.. image:: images/unity-editor-icon.png
   :class: center-image

----

:data-x: r2000
:data-y: r0

Google Daydream Technical Preview

 * `special preview build from unity <https://unity3d.com/partners/google/daydream>`_
 * Out of the box, basic functionality

*or* Google VR Plugin

 * Installer for Unity on `🍎+💻 <https://store.unity.com/>`_ (or `🐧 <http://forum.unity3d.com/threads/unity-on-linux-release-notes-and-known-issues.350256/>`_)
 * `Plugin <https://github.com/googlevr/gvr-unity-sdk>`_ gives full controller support and more
        
----

:class: hide-background

.. image:: images/unity-demo-new-project.png
   :class: center-image

.. note::
   Create a new Project

----

:class: hide-background

.. image:: images/unity-demo-new-project-wizard.png
   :class: center-image

.. note::
   Name it

----

:class: hide-background

.. image:: images/unity-demo-empty.png
   :class: center-image-huge

.. note::
   See it

----

:data-x: r0
:data-y: r-100
:data-scale: .6
:class: hide-background

.. note::
   Main stage: see everything important happening here

----

:data-x: r2000
:data-y: r100
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-new-plane-menu.png
   :class: center-image-huge

.. note::
   Populate stage: Add a plane

----

:data-x: r-500
:data-y: r-350
:data-scale: .3
:class: hide-background

.. note::
   Menu > GameObject > 3D Object > Plane

----

:data-x: r2500
:data-y: r350
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-new-plane-result.png
   :class: center-image-huge

.. note::
   Show GameObject Plane

----

:data-x: r2000
:data-y: r0
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-inspector.png
   :class: center-image-huge

.. note::
   Open inspector on righthand side

----

:data-x: r650
:data-y: r-200
:data-scale: .4
:class: hide-background

.. note::
   Search for ``Inspector >  Transform > Scale``

----

:data-x: r1350
:data-y: r200
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-plane-scaled.png
   :class: center-image-huge

.. note::
   * See size changed to be screen filling.
   * Let's make it more exciting > more objects!

----

:data-x: r2000
:data-y: r0
:class: hide-background

.. image:: images/unity-demo-new-objects-menu.png
   :class: center-image-huge

.. note::
   Let's add more objects

----

:data-x: r2000
:data-y: r0
:class: hide-background

.. image:: images/unity-demo-cube-added.png
   :class: center-image-huge

.. note::
   A Cube appears

----

:class: hide-background

.. image:: images/unity-demo-cube-moved.png
   :class: center-image-huge

.. note::
   Move that cube.

----

:data-x: r-50
:data-y: r-150
:data-scale: 0.25
:class: hide-background

.. note::
   Take a look where the mouse cursor is pointing at.

----

:data-x: r2050
:data-y: r150
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-more-objects-added.png
   :class: center-image-huge

.. note::
   Adding one of each: Cube/Sphere/Cylinder/Capsule

----

:data-x: r350
:data-y: r50
:data-scale: 0.25
:class: hide-background

.. note::
   Take a look at the camera preview: It does not look to colourfull. Let's change that.

----

:data-x: r1650
:data-y: r-50
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-assets.png
   :class: center-image-huge

.. note::
   Overview of next steps: Let's add materials.

----

:data-x: r-775
:data-y: r200
:data-scale: 0.2
:class: hide-background

.. note::
   Click on ``Favorites\All Material``

----

:data-x: r400
:data-y: r-50
:data-scale: 0.15
:class: hide-background

.. note::
   Click on ``Asset Store``

----

:data-x: r0
:data-y: r100
:class: hide-background

.. note::
   Click on an asset which is interesting/looks nice (``RedBeard_Bluestone WallV2``)

----

:data-x: r1000
:data-y: r-500
:data-scale: 0.5
:class: hide-background

.. note::
   * Check ``Asset count``: Defines how many different materials are included. the more the nicer looking.
   * Hit ``Import package``.

----

:data-x: r1375
:data-y: r150
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-assets-import-dialog.png
   :class: center-image

.. note::
   Hit ``import`` after checking all checkmarks (should already be the case)

----

:data-x: r2000
:data-y: r0
:class: hide-background

.. image:: images/unity-demo-multi-assign-material.png
   :class: center-image-huge

.. note::
   No change, we have to assign the material to different objects.

----

:data-x: r-150
:data-y: r-200
:data-scale: .3
:class: hide-background

.. note::
   Use SHIFT to click select multiple objects.

----

:data-x: r900
:data-y: r0
:class: hide-background

.. note::
   Hit the little hidden button next to ``Inspector > ✓ Mesh Renderer > Materials > Element 0 > Default Material … ○``

----

:data-x: r-1250
:data-y: r375
:class: hide-background

.. note::
   * Select a material to be used.
   * Repeat for all objects.

----

:data-x: r2500
:data-y: r-175
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-multi-material.png
   :class: center-image-huge

.. note::
   Looks nice, let's ``run`` it.

----

:data-x: r2000
:data-y: r-450
:data-scale: 0.2
:class: hide-background

.. note::
   * Run the current program to see what the user would see.
   * (comparable to deploying  it to an emulator, checking before deploying to phone)

----

:data-x: r0
:data-y: r450
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-play-no-rigid.png
   :class: center-image-huge

.. note::
   Looks nice, but there is nothing happening, let's change that!

----

:data-x: r2000
:data-y: r0
:class: hide-background

.. image:: images/unity-demo-rigid-menu.png
   :class: center-image-huge

.. note::
   Overview of adding a ``gravity`` animation

----

:data-x: r0
:data-y: r-270
:data-scale: 0.2
:class: hide-background

.. note::
   * Select all gravityable objects using SHIFT and left mouse click. 
   * Do not add the plane, since the other objects need something to ``land`` on.

----

:data-x: r-450
:data-y: r-100
:data-scale: 0.5
:class: hide-background

.. note::
   Add ``gravity`` to all selected objects by hitting menu option ``Component > Physics > Rigidbody``.

----

:data-x: r2450
:data-scale: 0.3
:class: hide-background

.. note::
   Hit play.

---- 

:data-x: r0
:data-y: r470
:data-scale: 1.0
:class: hide-background

.. image:: images/unity-demo-rigid-simple.gif
  :class: center-image-huge

.. note::
   * Show stupidly simple animation
   * Nice, but we can do more ....

----

:data-x: r2000
:data-y: r-70
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-rigid-complex.png
   :class: center-image-huge

.. note::
   * Copying objects by using ``Copy and Paste``
   * Also: I moved the camera inside of the action

----

:data-y: r0

:class: hide-background

.. image:: images/unity-demo-rigid-complex.gif
   :class: center-image-huge

.. note::
   * Now with fancy interactions and animations.
   * Cannot see the other parts, lets use a cardboard! :)

----

:class: hide-background

.. image:: images/unity-demo-add-gvr-menu.png
   :class: center-image-huge

.. note::
   Import the Unity package by going to Assets > Import Package > Custom Package.

----

:data-x: r-600
:data-y: r-300
:data-scale: 0.4
:class: hide-background

.. note::
   zoomed in view

----

:data-x: r2600
:data-y: r300
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-add-gvr-dialog.png
   :class: center-image

.. note::
   * Find the checked out folder from step 1
   * Select the ``GoogleVRForUnity.unitypackage``
   * Hit ``Open``.
   * Wait

----

:data-x: r2000
:data-y: r0
:class: hide-background

.. image:: images/unity-demo-add-gvr-all-packages.png
   :class: center-image-huge

.. note::
   Select ``all`` and hit ``ok`` again. You have now the complete sdk imported.

----

:data-x: r2000
:class: hide-background

.. image:: images/unity-demo-add-gvr-progress.png
   :class: center-image

.. note::
   Please wait ... ;)

----

:class: hide-background

.. image:: images/unity-demo-add-gvr-update.png
   :class: center-image

.. note::
   * Updating is fine for simple projects, more complex might be an issue.
   * ``I Made a Backup. Go Ahead!``

----

:class: hide-background

.. image:: images/unity-demo-add-gvr-add-gvrmainviewer.png
   :class: center-image-huge

.. note::
   * Sofar no changes
   * We need to add the ``GvrViewerMain`` to the camera of our scene.

----

:data-x: r-775
:data-y: r300
:data-scale: 0.3
:class: hide-background

.. note::
   Select ``Project > Assets > GoogleVR > Prefabs``

----

:data-x: r400
:data-y: r-100
:data-scale: 0.25
:class: hide-background

.. note::
   Start drag and drop the ``prefab``.

----

:data-x: r1675
:data-y: r-400
:data-scale: .3
:class: hide-background

.. note::
   * Drop it onto the Main Camera (indicated by round rect)
   * Sofar no changes
   * We need to add the ``GvrViewerMain`` to the camera of our scene.

----

:data-x: r700
:data-y: r400
:data-scale: 1
:class: hide-background

.. image:: images/unity-demo-add-gvr-dnd-camera.png
   :class: center-image-huge

.. note::
   * Again no change :(
   * Let's run it.

----

:data-x: r2000
:data-y: r0
:class: hide-background

.. image:: images/unity-demo-cardboard-simple.gif
   :class: center-image-huge

.. note::
   * We see changes
   * Image distortion, left and right eye
   * Can we simulate rotation of the head?

----

:class: hide-background

.. image:: images/unity-demo-cardboard-rotation.gif
   :class: center-image-huge

.. note::
   Yes, we can simulate by holding down ALT and moving the cursor.

----

Summary of Unity Demo 
---------------------

* Using Unity is fast
* Using Cardboard SDK is easy
* Using internal renderer for simulating
* ``GvrIntent`` start of interoperation Android - Unity

.. container:: center

   `📄 Project <http://bit.ly/mbvrvienna-git>`_ `📱 APK <https://bit.ly/mbvrvienna-apk>`_

----

Difficulties in using Unity
---------------------------

* Cost for non free version exists.
* Integration with other (Java) libraries difficult at best.

----

:data-x: 0
:data-y: r1300

.. image:: images/daydream-logo.png
   :class: center-image
   :width: 1000px

.. note::

        * Introduced at Google I/O this year.
        * Soon™ first hardware available.

----

:data-x: r2000
:data-y: r0

:class: hide-background

.. image:: images/daydream-headset.png
   :height: 800px

----

:class: hide-background
:data-x: r190
:data-y: r240
:data-scale: 0.2

.. note::
   Controller

   * uses special hardware as controller

     * can get emulated by any Android phone (>= 4.4)
     * has four Buttons: Volume +/-, App(Programmable), Home
     * clickable Touchpad. (x/y position, clicked state)(emulated by two touches)

   * Print out sheet to not get to disctracted by Phone
   * Connects via bluetooth to ``Headset Phone``

----

:class: hide-background
:data-x: r-400
:data-y: r-12
:data-scale: 0.3

.. note::
   Headset Phone

   * has to be a ``Nexus 6P`` running ``Android Nougat``
   * start a Daydream app once, set it up by clicking on the ``Gear``, enabling all VR settings
   * ``Reboot phone ...`` ;) .
   * Bluetooth to connect to controller.

----

:class: hide-background
:data-x: r210
:data-y: r-228
:data-scale: 0.5

.. note::
   Complete Package

   * ``Daydream Ready``

     * high performance sensors for high accuracy head tracking
     * displays with fast response time to minimize blur
     * powerfull mobile processor
     * VR System notifications

   * will be available ``in fall``
   * will be created by hardware partners
   * certified by ``Google``
   * Google Play for VR and ``Daydream Home``

----

:data-x: r2000
:data-y: r0
:data-scale: 1

Daydream SDK features
---------------------

* Same as Cardboard SDK
* Controlling the controller

  * orientation/acceleration 
  * input (Clickpad: x,y, clicked, App Button, Vol+/-)

* spatial audio engine

----


.. container:: center

  VrView on Web/iOS/Android

.. raw:: html

  <iframe width="100%" height="90%" allowfullscreen frameborder="0" src="https://storage.googleapis.com/vrview/index.html?image=https://raw.githubusercontent.com/google/vrview/master/examples/pano/andes_2048.jpg&is_stereo=true"></iframe>

.. note::
   VRView, available for 

   * Android
   * IOS
   * Web
   
   Not for Unity!

----

Simple RecyclerView with 4 VrViews `🎥 Images from Google <https://github.com/google/vrview>`_

.. image:: images/android-demo-final.gif
   :class: center-image

.. note::
   Final result of our current demo

----

:class: hide-background

.. image:: images/andes.jpg
   :class: center-image

.. note::
   Those images are represented by the ids seen earlier

----

Sample Recycler View Project
----------------------------

`📄  Source Code <http://bit.ly/mbvrvienna-android>`_

.. image:: images/android-demo-untouched.png
   :class: center-image

.. note:: 
   Using VrPanoramaView we'll be able to generate those interactions.

----

Project Layout
--------------

.. code:: bash
  
  MainActivity.java
  ConstantResourceAdapter.java

  activity_main.xml 
  resource_layout.xml 

----

MainActivity.java

.. container:: dimmed

 .. code:: java
  
  ButterKnife.bind(this);
  
  recyclerView.setLayoutManager(
    new LinearLayoutManager(this, 
      LinearLayoutManager.VERTICAL, false));

  RecyclerView.Adapter adapter = 
    new ConstantResourceAdapter();

  recyclerView.setAdapter(adapter);

.. note:: 
  Uses ``ButterKnife`` to bind ``activity_main.xml``'s ``RecyclerView``, 
  creates the ``ConstantResourceAdapter``.

----

MainActivity.java

.. code:: java
  
  ButterKnife.bind(this);
  
.. container:: dimmed

 .. code:: java
  
  recyclerView.setLayoutManager(
    new LinearLayoutManager(this, 
      LinearLayoutManager.VERTICAL, false));

  RecyclerView.Adapter adapter = 
    new ConstantResourceAdapter();

  recyclerView.setAdapter(adapter);

----

MainActivity.java

.. code:: java
  
  ButterKnife.bind(this);
  
  recyclerView.setLayoutManager(
    new LinearLayoutManager(this, 
      LinearLayoutManager.VERTICAL, false));

.. container:: dimmed

 .. code:: java
  
  RecyclerView.Adapter adapter = 
    new ConstantResourceAdapter();

  recyclerView.setAdapter(adapter);

----

MainActivity.java

.. code:: java
  
  ButterKnife.bind(this);
  
  recyclerView.setLayoutManager(
    new LinearLayoutManager(this, 
      LinearLayoutManager.VERTICAL, false));

  RecyclerView.Adapter adapter = 
    new ConstantResourceAdapter();

  recyclerView.setAdapter(adapter);

----


ConstantResourceAdapter.java

.. code:: java

  private static final List<Integer> elements = 
    new ArrayList<>();

  static {
    elements.add(R.drawable.andes);
    elements.add(R.drawable.congo);
    elements.add(R.drawable.coral);
    elements.add(R.drawable.io2016);
  }
    
----

ConstantResourceAdapter.java

.. code:: java

  static class ResourceItemViewHolder 
    extends RecyclerView.ViewHolder {
    private final TextView textView;

    public ResourceItemViewHolder(View itemView) {
      super(itemView);
      textView = (TextView) itemView;
    }
  }


----

ConstantResourceAdapter.java

.. container:: dimmed

 .. code:: java
  
  public 
  RecyclerView.ViewHolder onCreateViewHolder(…) {
    
    final LayoutInflater layoutInflater = 
      LayoutInflater.from(parent.getContext());
    
    final View inflate = 
      layoutInflater.inflate(R.layout.resource_layout,…
    
    return new ResourceItemViewHolder(inflate);
  }

----

ConstantResourceAdapter.java


.. code:: java
  
  public 
  RecyclerView.ViewHolder onCreateViewHolder(…) //{


.. container:: dimmed
 
 .. code:: java     
 
      final LayoutInflater layoutInflater = 
        LayoutInflater.from(parent.getContext());
    
      final View inflate = 
        layoutInflater.inflate(R.layout.resource_layout,…
    
      return new ResourceItemViewHolder(inflate);

.. code:: java
  
  }

----

ConstantResourceAdapter.java


.. code:: java
  
  public 
  RecyclerView.ViewHolder onCreateViewHolder(…) {

    final LayoutInflater layoutInflater = 
      LayoutInflater.from(parent.getContext());
    
    final View inflate = 
      layoutInflater.inflate(R.layout.resource_layout);}
  
.. container:: dimmed
 
 .. code:: java     
 
      return new ResourceItemViewHolder(inflate);

.. code:: java
  
  }

----

ConstantResourceAdapter.java


.. code:: java
  
  public 
  RecyclerView.ViewHolder onCreateViewHolder(…) {

    final LayoutInflater layoutInflater = 
      LayoutInflater.from(parent.getContext());
    
    final View inflate = 
      layoutInflater.inflate(R.layout.resource_layout,…)

    return new ResourceItemViewHolder(inflate);
  }

----

ConstantResourceAdapter.java

.. code:: java

  public void onBindViewHolder(
    RecyclerView.ViewHolder baseHolder, 
    int position) {
    
    final ResourceItemViewHolder viewHolder = 
      (ResourceItemViewHolder) baseHolder;
    
    viewHolder.textView.setText(
      elements.get(position));
  }

----

resource_layout.xml

.. code:: xml

  <TextView 
     […]
     android:layout_height="100dp"
     android:textSize="32sp"
   />

----

Result

.. image:: images/android-demo-untouched.png
      :class: center-image

----

Making the change
-----------------

Add \*.aar dependencies to app

 * `common.aar <https://github.com/googlevr/gvr-android-sdk/raw/master/libraries/common/common.aar>`_
 * `commonwidget.aar <https://github.com/googlevr/gvr-android-sdk/raw/master/libraries/commonwidget/commonwidget.aar>`_ and 
 * `panowidget.aar <https://github.com/googlevr/gvr-android-sdk/raw/master/libraries/panowidget/panowidget.aar>`_ 

from `Google VR Android Github <http://github.com/googlevr/gvr-android-sdk>`_ 

----

Change in ``resource_layout.xml``

.. code:: xml
  
  <TextView
    […]

to

.. code:: xml

  <com.google.vr.sdk.widgets.pano.VrPanoramaView
     […]

----

Change in ``ConstantResourceAdapter.java``

.. code:: java

    class ResourceItemViewHolder 
      extends RecyclerView.ViewHolder {
    
    private final VrPanoramaView vrPanoramaView;

    public ResourceItemViewHolder(View itemView) {
      super(itemView);
      vrPanoramaView = (VrPanoramaView) itemView;
    }
  }

.. note::
  Replacing  TextView with VrPanoramaView

----

.. code:: java
   
  @Override public void onBindViewHolder(…) //{

.. container:: dimmed

 .. code:: java

    final ResourceItemViewHolder viewHolder = 
      (ResourceItemViewHolder) baseHolder;
    final Resources resources = 
      viewHolder.vrPanoramaView.getResources();
    final Bitmap bitmap = 
      BitmapFactory.decodeResource(resources, 
        elements.get(position));
    viewHolder.vrPanoramaView
      .loadImageFromBitmap(bitmap, null);

.. code:: java 

  }

----

.. code:: java
   
  @Override public void onBindViewHolder(…) //{

    final ResourceItemViewHolder viewHolder = 
      (ResourceItemViewHolder) baseHolder;
.. container:: dimmed

 .. code:: java

    final Resources resources = 
      viewHolder.vrPanoramaView.getResources();
    final Bitmap bitmap = 
      BitmapFactory.decodeResource(resources, 
        elements.get(position));
    viewHolder.vrPanoramaView
      .loadImageFromBitmap(bitmap, null);

.. code:: java 

  }

----

.. code:: java
   
  @Override public void onBindViewHolder(…) //{

    final ResourceItemViewHolder viewHolder = 
      (ResourceItemViewHolder) baseHolder;
    final Resources resources = 
      viewHolder.vrPanoramaView.getResources();
.. container:: dimmed

 .. code:: java
    
    final Bitmap bitmap = 
      BitmapFactory.decodeResource(resources, 
        elements.get(position));
    viewHolder.vrPanoramaView
      .loadImageFromBitmap(bitmap, null);

.. code:: java 

  }

----

.. code:: java
   
  @Override public void onBindViewHolder(…) //{

    final ResourceItemViewHolder viewHolder = 
      (ResourceItemViewHolder) baseHolder;
    final Resources resources = 
      viewHolder.vrPanoramaView.getResources();
    final Bitmap bitmap = 
      BitmapFactory.decodeResource(resources, 
        elements.get(position));
.. container:: dimmed

 .. code:: java

    viewHolder.vrPanoramaView
      .loadImageFromBitmap(bitmap, null);

.. code:: java 

  }

----

.. code:: java
   
  @Override public void onBindViewHolder(…) //{

    final ResourceItemViewHolder viewHolder = 
      (ResourceItemViewHolder) baseHolder;
    final Resources resources = 
      viewHolder.vrPanoramaView.getResources();
    final Bitmap bitmap = 
      BitmapFactory.decodeResource(resources, 
        elements.get(position));
    viewHolder.vrPanoramaView
      .loadImageFromBitmap(bitmap, null);
  }

----

Result

.. image:: images/android-demo-final.gif
   :class: center-image

.. note::
   Final result of our current demo

----

What did we do?
---------------

* Loaded a equirectangular image into a bitmap
* Let it be displayed by a `VrPanoramaView`
* Use Daydream SDK to display it

----

Limitations of Daydream for Android SDK
---------------------------------------

* using 3D models has to be done by

  * either low level OpenGL or 
  * 3rd party 3d engine

----

:data-x: 10000
:data-y: 7500
:data-z: 0
:data-scale: 12
:class: last-slide

What will you build?
--------------------

.. container:: center

  `🎥 General <https://youtu.be/rOCaujUOCuE>`_ `🎥 Controller <https://www.youtube.com/watch?v=l9OfmWnqR0M>`_ `🎥 Designing <https://www.youtube.com/watch?v=00vzW2-PvvE>`_

.. container:: center

  `📄 Google VR <https://vr.google.com>`_ `Github <https://github.com/googlevr/gvr-android-sdk>`_

.. container:: center

  `🐦@MarioBodemann <http://twitter.com/@MarioBodemann>`_

