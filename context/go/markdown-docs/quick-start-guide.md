## Getting Started With Noctua and LEGO Curation

* What is LEGO?
* What is Noctua?
* Creating a LEGO Model
 * Login
 * Accessing the Graph Editor
 * Creating an Individual
 * Adding Contextual Information
 * Adding Evidence
 * Linking Individuals
 * Naming your Model and Saving your Work
* Incorporating LEGO Annotations into your Workflow

### What is LEGO?

LEGO (Linked Expressions using the Gene Ontology) is a formalism for
constructing models of biological pathways or processes using Gene
Ontology (GO) annotations, contextual information (e.g., cell and
tissue types) and defined semantic relations from the Relations
Ontology (RO).

### What is Noctua?

Noctua (http://noctua.berkeleybop.org) is the web-based collaborative
editing system used to create LEGO models. Noctua can also be used to
create simpler, conventional GO annotations that may be incorporated
into LEGO models.

### Creating a LEGO Model

#### Login

To create or edit a LEGO model using Noctua, you currently need to
have two things: an email address registered with
[Persona](http://persona.org) and to be properly registered as a
Noctua user in the GO users' metadata for that email address. If you
are already a registered GO curator and have a Persona account, you
can login to Noctua by following the steps after clicking [Login] on
any page and be clicking [Return] once a token has been issued.

If you don't already have a [Persona](http://persona.org) account, as
long as you have a public email address, you can register the first
time you try to login. The more important step is to get your
information properly into the users' metadata file. The easiest way to
do this is to fill out the online
[new user form](http://bit.ly/new-noctua-user) and contact sjcarbon at
lbl dot gov once complete. Propagating the metadata information may
take a little time, so please do this as early as possible. To fill
out this form, you will need your name, organization, and ORCID (yes,
you'll need one of those as well if you do not have one).

Please note that in many browsers you must have pop-up blocking disabled
for the Noctua domains in order to be able to get the login dialog.

#### Accessing the Graph Editor

Once you've logged into Noctua, click on the [Create Noctua
Model] button at the top of the home page to create a new model using
graphical editing interface. If you want to edit an existing model,
click on the "Edit" button to the right of that model in the list at the
bottom of the page.

#### Creating an Individual

The core graphical view of a statement in LEGO is called an
"individual". To create a new individual, you can click on either of
the four options on the left side of the editor: [Add individual],
[Add annoton], [Add function], [Add process]. Simply fill in the the
autocomplete fields in one of the options and hit the appropriate
"add" button. The core unit of annotation for a LEGO model is the
annoton. Annotons represent linked statements about the function of a
gene product, where the function occurs at a cellular level and the
process in which the function is executed.

*Add text and screenshot for each.*

#### Adding Contextual Information

Information about an individual, for example a statement that a
Molecular Function is enabled by a given entity, can be refined by
adding additional contextual information such as input for the
Molecular Function. To add contextual information to an individual,
click on the green box in the individual and in the resulting pop-up
window go to the section entitled "Add edge & class expression" and
enter the appropriate relation and entity in each of the two
respective fields.

#### Adding Evidence

Every assertion in a LEGO model should be supported by evidence. To
add evidence to an individual, click on the empty box in the upper
right corner of each colored box that illustrates a relation and an
entity. In the resulting pop-up window, go to the "Evidence" section
and add an Evidence Code from the Evidence Code Ontology (ECO), a
supporting reference (either PMID, doi, or GO\_REF), and where
appropriate an entry in the With/From field.

#### Linking Individuals with Relations

Individuals in LEGO models are linked with semantically
appropriate relations from the RO. To link two individuals, click on
the blue circle in the box of the individual that is the "subject" of
the relation and drag the cursor from that individual to the individual
that is the "object" of the relation. The "object" individual will be
highlighted when you've made the connection and then a pop-up window
will open displaying a list of RO relations. Click on the radio button
for the relation you want to use and then save your selection. The
evidence pop-up window is searchable in the standard ways for searching
a web page.

To add evidence to a relation, click on the box containing the
relation name and you will be taken to a pop-window where you can add an
Evidence Code, reference, and With/From entry, as described above.

To delete a relation, drag the blue circle off of the "object"
individual and onto the background canvas. The relation will
automatically be deleted from your model.

#### Naming your Model and Saving your Work

While you create or edit your model, you will see an asterisk appear
around the "Untitled" text in your browser tab. The asterisk indicates
that your work is not yet saved, and the "Untitled" indicates that you
have not yet named your model. To name your model and save your work,
click on the drop-down menu under the Model heading and select the
"Edit Annotations" option. In the "Title" section, add a title for
your model. The beginning of the title will now appear in the browser
tab. To save your work, click on the Model heading again and select
the "Save" option. Your work is now saved and the asterisk in the tab
will disappear. Save your work often while editing!

#### How to Make a Model Public

LEGO models can exist in different curation states, depending
upon whether the curator(s) wish to make the model public. This allows
curators to work on a model over a period of time, perhaps review them
with colleagues or experts in the field, and then publish them to the GO
or other web sites.

By default, new models are treated as if they are under
development, but curators have the ability to explicitly label the
production status of their model. To do this, click on the Model drop
down menu and select "Edit Annotations" from the list. Under the
"Annotation state" section, select from one of five options:

* Production - model will be available from viewing on the GO web site and annotation files available on Jenkins (see below)
* Review 
* Development - model is still being curated and is not available for viewing on the GO web site; annotations cannot be retrieved from Jenkins (see below)
* Closed
* Delete

### Incorporating LEGO Annotations into your Workflow

GO annotations created in Noctua can be downloaded in three
different annotation file formats: GAF, GPAD, and OWL.  Note that the
OWL representation of LEGO models is the semantically correct
representation, and that GAF and GPAD file formats are the closest
representation of the OWL-based LEGO model that can be made using these
legacy annotations file formats.

From Noctua, annotation files for a specific model can be viewed
and downloaded by clicking on the Model drop down and then selecting the
appropriate Export option from the list. Resulting annotation files
will appear in the browser and can be downloaded from there.

Alternatively, LEGO annotations files can be retrieved from
Jenkins. Currently there is a repository for legacy file formats that
are marked production
[here](http://build.berkeleybop.org/view/GO/job/export-lego-to-legacy/).

OWL models may be retrieved here:

*TBD.*