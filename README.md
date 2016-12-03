Cyclone: A set of Pure Data objects cloned from Max/MSP 
-------

> Cyclone expands Pure Data with objects cloned from cycling74's Max/MSP. It thus provides some level of compatibility between the two environments, helping users of both systems in the development of equivalent patches. 

--------------------

Pure Data (or just "Pd") project is found at: https://sourceforge.net/p/pure-data/pure-data/ci/master/tree/

Max is found at: https://cycling74.com/

--------------------

<strong>Exerpt from Cyclone's original Readme:</strong>

"Cyclone is a library of Pure Data classes, bringing some level of compatibility between Max/MSP and Pd environments. Although being itself in the early stage of development, it is meant to eventually become part of a much larger project, aiming at unification and standardization of computer musician's tools. 

In its current form, cyclone is mainly for people using both Max and Pd, and thus wanting to develop cross-platform patches. (...)."

The full original readme is provided in this repository at: <https://github.com/porres/pd-cyclone/blob/master/maintenance/README_original.txt>

-------

<strong>History of cyclone's maintenance up to the present day:</strong>

Cyclone's original author is Krzysztof Czaja, who worked on it as part of his miXed library from 2002 to 2005 and later abandoned it all together. 

In parallel, miXed had been incorporated into into Pd Extended, so (after abandoned by Czaja) it was eventually under the maintenance of Hans-Christoph Steiner - the main developer and maintainer of the Pd-Extended. 

Pd Extended was abandined after its latest release (in jan-2013), Cyclone was left unmaintained as a result until Fred Jan Kraan took over maintainance and development for cyclone in dec-2014. In feb-2016, Fred Jan decided to abandone development for cyclone, though maintenance for his last package is still active. 

Since feb-2016, an active further development of cyclone is being proposed by Alexandre Porres & collaborators (mainly Derek Kwan and Matt Barber) on this repository.

-------

<strong>About earlier versions and other repositories:</strong>

There are two other cyclone repositories, here's some info about them and the earlier versions of cyclone.

=> <strong>Original Repository (up to version 0.1-Alpha-57):</strong>
Cyclone is originally part of the miXed library (also written by cyclone's original author Krzysztof Czaja). The original repository of MiXed as part of Pd Extended - containing cyclone and more (such as 'toxy') - resides at <https://svn.code.sf.net/p/pure-data/svn/trunk/externals/miXed/cyclone> and the migrated repository: <https://git.puredata.info/cgit/svn2git/libraries/miXed.git/>. 

- <strong>Czaja's era (up to 0.1-Alpha55):</strong> Cjaza worked on cyclone from alpha01 (2002) to alpha55 (2005). 

- <strong>Hans era (0.1-Alpha-55 and 0.1-Alpha-56):</strong> Hans maintained cyclone from 2005 to 2013. The 0.1-Alpha55 version of cyclone is found in most of Pd-Extended versions up to Pd-Extended 0.42-5. The last release of Pd-Extended is 0.43.4 from jan-2013 and it carries the 0.1-Alpha56 version of cyclone, which can also be found as "cyclone-v0-0extended" when searching for externals in Pd Vanilla (since Pd Vanilla 0.47-0).

- <strong>Fred Maintenance era (0.1-Alpha-57):</strong> The last version currently found in the original cyclone repository is 0.1-alpha-57, which was developed by Fred Jan Kraan, who started maintaining cyclone in dec 2014. Although a compiled version for this version was made available at some point, it is not found there anymore and it is officially an "unreleased" version.

=> <strong>Fred Jan Kraan's Repository (0.1-Alpha-57 and 0.2beta):</strong> Fred Jan Kraan forked the original repository to <https://github.com/electrickery/pd-miXedSon>, but containing only the cyclone library. This repository starts with the last snapshot of the original cyclone repository: cyclone version 0.1alpha-57, from october 2015 (found in: <http://puredata.info/downloads/cyclone/releases/0.1-alpha57>).

- <strong>Cyclone 0.2-beta:</strong> Cyclone "0.2beta" presents further development on Fred Jan's branch, not available in the original repository. This is the last released version of cyclone available. It is found in Fred Jan Kraan's repository and also when searching for externals in the latest Pd Vanilla - check https://github.com/electrickery/pd-miXedSon/releases

-------

<strong>About this repository and its Goals:</strong>

Location of this repository is: https://github.com/porres/pd-cyclone. 

Porres forked cyclone in its last 0.2beta1 state to this new repository. When cyclone was been left unmaintained (in february 21st 2016), further developments for cyclone have been in the makings here since then.

This repository is faithful to the original goal of cyclone in creating an external Pd package with a collection of objects cloned and compatible to Max/MSP objects, which is a ground rule manifested by Hans-Christoph Steiner on the Pd-List about further maintenance of cyclone.

Cyclone was originally developed in Max/MSP 4 era but was still missing functionalities  - 


- Cyclone's original development starts in 2002 (at the time of Max 4.0) and is abandoned in 2005 with updates after Max 4.0 that never made it into the project. Further developments in cyclone were also not able to fully meet a compliance to the latest Max 4 release (Max 4.6.3 from 2007). Moreover, Max has also introduced new functionalities on some objects in the more recent versions (from Max 5 to Max 7). The cyclone version at the time we forked (0.2beta1) is still mostly outdated to Max/MSP 4, with minor exceptions that include functionalities introduced in Max 5 (but still missing functionalities from Max 6 and Max 7 versions). 

If in agreement to the Pd community, this repository will release an update of the cyclone project (version 0.3). If so be it, besides bug fixes in current existing objects, new/further developments in cyclone 0.3 shall include:

<strong>- A)</strong> Update cyclone to include missing functionalities from Max 4 up to the latest Max version (currently Max 7.3.1) into the already existing objects in cyclone.

<strong>- B)</strong> New objects compatible to the latest Max version. 

Such an update represents the major overhaul since the original author abandoned cyclone in 2005. With such a great deal of work, this repository/project is open to collaboration to anyone who wishes to work according to the key and central goal of Max/MSP compatibility. Ideally, any possible Max/MSP object could be cloned or updated, but since this is a fair amount of work, collaborators are free to decide and work on what they consider more relevant and important. Any object that has full or "most possible" compatibility to current Max/MSP can be included. 

Some collaborators are already helping coding new objects and updating/fixing old ones, a list of known bugs and things "to do" will be made available with the first release to come from this repository.

Check some stuff we've been doing in our changelog: https://github.com/porres/pd-cyclone/wiki/cyclone-0.3-changlelog

This Readme file was created on February 22nd 2016 
(last edited on December 3rd 2016)

-------
<strong>Building Cyclone:</strong>

When Fred Jan Kraan forked to his repository and worked on the release of cyclone 0.1-alpha57, the cyclone package has started relying on the new build system called "pd-lib-builder" by Katja Vetter (check the project in: <https://github.com/pure-data/pd-lib-builder>). 

With this new build system, all you have to do is have the latest pd vanilla installed and type "make" in your compiler to build cyclone for your platform.

* Compiling with pdlibbuilder

PdLibBuilder tries to find the Pd source directory at several common locations, but when this fails, yo have to specify the path yourself using the pdincludepath variable. Example:

<pre>make pdincludepath=~/pd-0.46-6/src/  (for Windows/MinGW add 'pdbinpath=~/pd-0.46-6/bin/)</pre>

* Installing with pdlibbuilder

The default path for installing might not be the best, surely for testing. Use the pkglibdir variable for this. Example:

<pre>make install pkglibdir=~/pd-externals/</pre>
