==============================
Marketing automation campaigns
==============================

The Odoo *Marketing Automation* app automates a variety of marketing tasks by combining specific
rules and filters to generate timed actions. Instead of manually having to build each stage of a
campaign (like a series of timed massmails), the *Marketing Automation* app allows marketers to
build the entire campaign, and all of its stages, in one place -- on one dashboard.

Campaign configuration
======================

To create a new automated marketing campaign, navigate to :menuselection:`Marketing Automation app
--> New` to reveal a blank campaign detail form.

.. image:: first_campaign/blank-marketing-campaign-form.png
   :align: center
   :alt: A blank marketing automation campaign form in Odoo Marketing Automation application.

After entering a name for the marketing campaign, configure the target audience in the remaining
fields.

A target audience can be configured by entering specific criteria for Odoo to use when determining
to whom this marketing automation campaign should be sent. Creating specific target audiences can
help businesses deliver tailored messages and campaigns that appeal to a niche demographic, thus
providing more value and personalization to all subsequent communications.

In the :guilabel:`Target` field, use the drop-down menu to choose which model the target audience
filters should be based on (e.g. :guilabel:`Contact`, :guilabel:`Lead/Opportunity`,
:guilabel:`Sales Order`, etc.).

Select :guilabel:`Search More...` from the drop-down menu to reveal a :guilabel:`Search: Target`
pop-up window containing all 157 target options.

Once a :guilabel:`Target` is selected, there's a :guilabel:`Unicity based on` field. This field is
used to avoid duplicates based on the model chosen in the :guilabel:`Target` field.

.. example::
   If :guilabel:`Customers` is chosen as the :guilabel:`Target`, select :guilabel:`Email` in the
   :guilabel:`Unicity based on` field so Odoo doesn't process any records that have the same Email
   address.

Select :guilabel:`Search More...` from the :guilabel:`Unicity based on` drop-down menu to reveal all
129 options in a pop-up window.

Lastly on the campaign detail form is the :guilabel:`Filter` field. This is where a more specific
audience filter can be configured to add specificity to the recipients of the marketing automation
campaign.

If left alone, the :guilabel:`Filter` field reads: :guilabel:`Match **all records**`. That means
Odoo uses the :guilabel:`Target` and :guilabel:`Unicity based on` fields to determine who the
recipients will be. The number of recipients is represented beneath as :guilabel:`record(s)`.

Campaign filter rules
---------------------

To add a more specific filter to a marketing automation campaign, click the :guilabel:`Add
condition` button in the :guilabel:`Filter` field. Doing so reveals a series of other configurable
filter rule fields.

In the rule fields, custom equations can be configured for Odoo to use when filtering who to include
or exclude in this specific marketing campaign.

.. image:: first_campaign/filter-node-equation-fields.png
   :align: center
   :alt: How the filter rule equation fields look in Odoo Marketing Automation campaigns.

.. note::
   :guilabel:`Records` represent the number of contacts in the system that fit the specified
   criteria for a campaign.

Also, once :guilabel:`Add condition` is clicked, the ability to :guilabel:`Save as
Favorite Filter` becomes available on the campaign form.

.. image:: first_campaign/save-favorite-filter-option.png
   :align: center
   :alt: How the Save as Favorite Filter option looks on marketing automation campaign form.

There is also the option to match records with :guilabel:`all` or :guilabel:`any` of the rules
configured in the :guilabel:`Filter` field. To choose either of those options, click :guilabel:`all`
from the middle of the sentence: :guilabel:`Match records with **all** of the following rules:` to
reveal a drop-down menu with those options.

.. image:: first_campaign/match-all-any-rules-drop-down.png
   :align: center
   :alt: Match records with all or any of the rules in Filter field for marketing campaigns.

When the first field of the rule equation is clicked, a nested drop-down menu of options appears on
the screen where specific criteria is chosen based on needs of the campaign. The remaining fields on
the rule equation further define the criteria, which is used to determine which records on the
database to include or exclude in the execution of the campaign.

To add another rule, either click the :guilabel:`➕ (plus sign)` icon to the right of the filtering
rule. Or click :guilabel:`New Rule` beneath the rule equation fields. When either are clicked, a new
series of rule fields appears.

To add a branch of multiple rules at the same time, click the :guilabel:`branch` icon, located to
the right of the :guilabel:`➕ (plus sign)` icon. When clicked, two additional sub-rule equation
fields appear beneath the initial rule.

.. image:: first_campaign/rule-branch-filter-sample.png
   :align: center
   :alt: Sample of how the rule branches look in the filter section of a marketing campaign.

There is also the option to have the filter apply to :guilabel:`any` or :guilabel:`all` of the
configured branch rules.

For further information on marketing automation campaign filter configuration, refer to :doc:`this
documentation page <target_audience>`.

.. seealso::
   - :doc:`workflow_activities`
   - :doc:`testing_running`
