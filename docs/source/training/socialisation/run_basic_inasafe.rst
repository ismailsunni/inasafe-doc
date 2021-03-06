.. _run-basic-inasafe:

Run Basic |project_name|
========================

**Objectives:**

* To run |project_name| using a flood model & population and examine the
  results
* To create a impact map
* To modify the threshold of an impact function
* To run |project_name| using a flood model & building and examine the results

**Expected Results:**

Participants are able to:

* run and understand the results of an |project_name| using a flood model &
  population
* create an impact map using the |project_name| print button
* change the threshold of an impact function
* run and understand the results of an |project_name| using a flood model &
  building

**Data for Practical**
You can download the InaSAFEv2.0.zip from `InaSAFE Training Data Packages
<https://data.inasafe.org/TrainingDataPackages/>`_
or it will be provided to you during the training.

Introduction
------------

In this chapter you will run |project_name| in Jakarta to determine the
impact of a flood model on both Jakarta's population and buildings.

1. :menuselection:`File --> Open Projects`

2. A message box appears: *Do you want to save the current project?*
   :guilabel:`Don't Save`

.. image:: /static/training/socialisation/028_saveproject.*
   :align: center

3. :guilabel:`Navigate` to the *InaSAFE_project* folder and :guilabel:`Select`
	 *Jakarta_floods.qgs*, :guilabel:`Open`

The result of opening the project:

.. image:: /static/training/socialisation/029_jakartafloods.*
   :align: center


People need evacuating
----------------------

As you can see the |project_name| panel has the first three drop down menus
filled in already:

* a flood similar to the 2007 Jakarta event
* buildings
* Be Flooded

4. In the |project_name| panel :guilabel:`Click` on buildings,
:guilabel:`Select` people, it now should have:

* a flood similar to the 2007 Jakarta event
* people
* Need evacuating

.. image:: /static/training/socialisation/030_showpeople.*
   :align: center

.. note:: You can see that the Impact function below **Might** automatically
   changed from *Be Flooded* to *Need evacuation* this is dependant on the
   combination of the hazard and exposure layers

5. Lets run this scenario first - :guilabel:`Run` at the bottom right
   hand corner of the |project_name| panel.

.. image:: /static/training/socialisation/031_run.png
   :align: center

A new layer should appear in the layer panel called *Population which needs
evacuating*

.. image:: /static/training/socialisation/032_results.*
   :align: center

In the |project_name| Panel, inside the main window you will see text and
statistics, lets explore this further.

.. image:: /static/training/socialisation/033_peoplefloodresult.*
   :align: center

**Evacuation:** There are 1,109,000 people that are located in water deeper than
1 meter. It is assumed that all of these people will need to evacuate their
homes.  The threshold of 1 meter can be changed (see Changing Threshold below).

**Minimum needs:** is calculated using the above number of evacuated people to
estimate the amount of food, water and other products that the refugees will
need to survive.  The figures are based on an Indonesian policy.

**Action checklist:** designed to make disaster managers think about what
they need to do to prepare for the event.

**Notes:** explains the total people in the map canvas, the threshold of water
depth that requires evacuation and the source of the minimum needs assessment.

**Detailed gender and age report:** Statistical breakdown of the number of
females, and added minimum needs for women hygiene and pregnant women. As
well as statistical breakdown of Youth, Adults and Elderly.

**Source:** where the exposure and hazard data originally came from.

Print Results
.............

.. note:: You can choose whether you want print the whole analysis or current
   extent. You also can pick print template or you can navigate to your own
   QGIS template (.qpt). For more information about printing Click
   :guilabel:`Help` in the print window.

6. :guilabel:`Print` at the bottom the |project_name| panel

.. image:: /static/training/socialisation/034_print.*
   :align: center

7. A window will pop up, ensure **Area of print** = Analysis extent and
   **Template to use** = inasafe. :guilabel:`Open PDF`

.. image:: /static/training/socialisation/034a_impact_report.*
   :align: center

8. Navigate to where you would like to save the pdf,
   and type :kbd:`Jakartaflood_evacuation_1m` :guilabel:`Save`

.. image:: /static/training/socialisation/034b_save_report.*
   :align: center

Two PDFs will be generated

.. note:: The result provides a map and a table of information about the impact.

.. image:: /static/training/socialisation/035_People_in_need_of_evacuation_1m.*
   :align: center

.. note:: In the new version of |project_name| the developers will look more
   into the layout of these pdfs. *If you get time during this course please
   proved us with your ideas on how the print map and table should look!*

Changing threshold
..................

What if the disaster manager has decided that people should be evacuated if they
are in 80cm or more of water?

9. :guilabel:`Show question form` found at the top of the |project_name| panel.

.. image:: /static/training/socialisation/036_showquestion.*
   :align: center

10. To change the impact function select :guilabel:`...` *Configure Impact
Function Parameter* which is found beside the *Need evacuation*

.. image:: /static/training/socialisation/037_functionchange.*
   :align: center

11. Type :kbd:`0.8` in the window

.. image:: /static/training/socialisation/038_configure.*
   :align: center

12. :guilabel:`OK`


13. :guilabel:`Run` |project_name|

.. image:: /static/training/socialisation/031_run.*
   :align: center

How have the numbers changed?

.. todo:: How many people need to be evacuated?
   **Answer:** ______________________
   Is this the answer you were expecting?
   **Answer:** _____________________

14. :guilabel:`Print` at the bottom the |project_name| panel

.. image:: /static/training/socialisation/034_print.*
   :align: center

15. A window will pop up, ensure **Area of print** = Analysis extent and
**Template to use** = inasafe. :guilabel:`Open PDF`

.. image:: /static/training/socialisation/034a_impact_report.*
   :align: center

16. Navigate to where you would like to save the pdf,
and type :kbd:`Jakartaflood_evacuation_80cm` :guilabel:`Save`

17. Before moving onto buildings, lets turn some layers off. In your Layer
panel you will now have 5 layers, we are going to uncheck everything but:

* a flood similar to the 2007 Jakarta event
* buildings

.. image:: /static/training/socialisation/039_buildingflood.*
   :align: center

Buildings Affected
------------------

18. Confirm that the |project_name| panel is the same as the image below

.. image:: /static/training/socialisation/040_inasafebuidlingflood.png
   :align: center

19. Notice that if you click on the *building* the people option is not
available, this is because *people* is not checked in the **Layer List**.

.. note:: If you want to be able to select layers within the
   |project_name| panel that are not checked in the **Layer List** you can
   modify the |project_name| options.
   For more information :doc:`../../user-docs/application-help/options`.
   We will also go through the option menu in :doc:`helpful_hints_and_tips`

20. :guilabel:`Run` the new combination.

.. image:: /static/training/socialisation/041_buildingfloodresults.png
   :align: center

In this scenario approximately 1,434 buildings could be effected out of 31,515
buildings.

Due to the provincial BPBD work in OpenStreetMap they have mapped all
important building (and then sum!).

Important buildings are defined as:

* Clinic/doctors
* Fire stations
* Government
* Hospitals
* Place of Worship
* Police stations
* Residential
* Schools
* Sports Facilities
* Univeristy/college

**Action Checklist:** A different set of Actions have been identified to
relate to structures.

**Note:** Similar to the last |project_name| analysis, this analysis also
assumes impact is in water above 1 meter.

**Detailed building type report:** This is a breakdown of important
infrastructure, when you choose to aggregate (we will do this later) this
table will show the number of buildings by aggregation boundary.

**Source:** of the Hazard and Population Datasets


21. :guilabel:`Print` at the bottom the |project_name| panel

.. image:: /static/training/socialisation/034_print.png
   :align: center

22. A window will pop up, ensure **Area of print** = Analysis extent and
**Template to use** = inasafe. :guilabel:`Open PDF`

.. image:: /static/training/socialisation/034a_impact_report.*
   :align: center

23. Navigate to where you would like to save the pdf,
and type :kbd:`Jakartaflood_inundated_1m` :guilabel:`Save`



Optional - Change the threshold to 0.8
......................................

24. Check that |project_name| has the following in the drop-down boxes

* a flood similar to the 2007 Jakarta event
* buildings
* Be Flooded

25. To configures the impact function select :guilabel: `...` *Configure Impact
Function Parameter* which is found beside the *Be flooded*

26. Type :kbd:`0.8` in the window

27. |project_name| :guilabel:`Run`

28. |project_name| :guilabel:`Print` and save accordingly

