Filters
=======

Filters in OpenCravat/OakVar allow to select those variants which are relevant. As the number of variants in a genome usually is very large, you need to filter them first. OpenCravat cannot load more than 100,000 variants at once.

Filter tab
----------

Select the **Filter** tab in the Result Viewer. There are the following sections:

•Samples

This is for oncological samples and is not used in Just-DNA-Seq.

•Genes

Here you can type in any particular gene names, one per line. Also you can load them from a file by clicking **Browse...**

•Variant properties

This section has 2 subtabs in its turn:

••Smart Filters

Here are various useful filters:

**Population AF «==***

**Sequence Ontology**

**Chromosome**

**Coding**

**ClinGen**

**ClinVar**

**dbSNP Common ID**

**Revel Rank Score >=**

**SIFT Prediction**

••Query Builder

Here you can create a set of filter rules.

By default, an opening (left) parenthesis appears with buttons **+** and **(** in the lower left corner, and a greyed out switch **NOT** appears if you hover the mouse in the upper left corner, which allows to make the following rule negative by clicking on it. Clicking **NOT** once again deactivates it.

Click **+** to add a rule. A line of boxes will appear:

The first drop-down box is the source to which the rule will apply. For example: Variant Annotation, ClinVar, PharmGKB etc.
The second drop-down box allow to select an item in the source to apply the rule. E.g. UID, Chrom, Position, Gene etc.
The following switch "not", greyed out (inactive) by default, allows to select if the following condition should apply or should not apply. For the latter, click the word "not", and it will become black (active). To remove "not" from the condition, just click it again, and it will be greyed out.
The next drop-down allows to select the condition from one of the following:
**has data** - if the item being searched contains any data
**equals** - opens one more box where you can enter what the item should be equal to
**is empty** - if the item being searched is empty
**in range** - opens two boxes where you enter the boundaries of the range where the item should be
**<=** - if the item is less or equal to the value in the following box
**>=** - if the item is greater or equal to the value in the following box
At the end of the line, a small "x" allows to delete the whole rule by clicking on it.

If you click **+** once again, another rule is added, and between them the operator **and** is displayed by default, meaning that to satisfy the filter, both rules should apply. You can change it to **or** by clicking on it, so that to satisfy the filter, one of rules being true may be enough. Clicking **or** once again turns it to **and** again.

You can add as many rules as you wish, and the operators **and** / **or** between them will follow the general priority logic of boolean operations, i.e. **and** has the priority over **or**, as in any program code.

To change the priority and build more complex logical rules, you can click **(** which makes a separate set of rules (in parentheses), which have higher priority, as in mathematical operations. Note than the **and** / **or** operator which appears before the parentheses depends of the previous operator selected, i.e. if it was **or**, the next one will also be **or**, and vice versa. You can always change the operators by clicking on them.

Within the parentheses, you can create any number of rules, and there are separate **+** and **(** buttons to add new rules and nested parentheses inside the parentheses. Also in the upper left corner a separate **NOT** switch appears if you hover the mouse over it.

You can also move any rule to another rule. To do this, drag an anchor **||** which appears from the left side of the rule if you hover the mouse there, and drop it on any rounded **+** anchors which appear between rules and/or parentheses (not on the **+** button that adds rules).

**BUG: if dropping a rule on certain location, it redirects browser to an error page**

Clearing Filters
----------------

Under any section you can click the **Clear** button to remove any filter settings from that section.

Applying the Filter
-------------------

When you finish building the filter, click **Apply Filter** in the lower right corner of the page. The number of variants in the lower left corner (the first number before the slash, while the second one is the total number of variants and is not changed) should now become smaller. These numbers also appear in the **FILTER** tab header, making it e.g. **FILTER 22/4,727,413**. If the number is small enough, you can switch to the **VARIANT** tab, or make the filter more strict to reduce the number.

Saving and Importing Filters
----------------------------

You can save the filter (the whole set of rules) in OpenCravat/OakVar for further loading, as well as exporting to a file, or import it from a file.

To save the filter, click the floppy disk icon in the lower right corner of the page, and enter the name.

**NOTE:** Filters are saved internally in OpenCravat/OakVar, i.e. on the server if using a remote installation. To have a filter saved into a local file, export it after saving.

The saved filter appears in the left part of the page in the **Saved Filters** list.
To load a saved filter, just click its name.
To export a saved filter into a file, click the icon with a down arrow next to its name.
To delete a saved filter, click the X icon in its line.

To import a filter from a file, click the "up error" (rightmost) button in the lower right corner of the page, and browse for a file to import (e.g. pathogenic.json). Clicking **Open** in the browse window loads the filter. **NOTE:** the filter is not saved automatically, you need to save it with "Save filter" (floppy) icon if you want to save in on the server for further working.
