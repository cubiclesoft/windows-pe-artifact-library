Windows PE Artifact Library
===========================

An artifact library containing files in the Windows Portable Executable file format (EXEs, DLLs, etc) for research and analysis purposes only.  This repository contains over 375 samples of nearly every possible type of PE file found in the wild.  Looking for samples of common and/or esoteric PE files for your PE file format project?  This repo probably has what you are looking for.

Artifacts in this library were found automatically via the artifact finder tool in the [Windows PE File Tools for PHP](https://github.com/cubiclesoft/php-winpefile) which selected these samples from over 60,000 scanned files.  Also relevant is [the dynamic ruleset used to find and name artifacts](https://github.com/cubiclesoft/php-winpefile/blob/master/support/artifact_rules.php).

Unusual license alert:  The binaries in this repo are NOT owned by CubicleSoft and each one has its own unique license when acquired as a formal binary file rather than as a PE file data sample.  This repository is intended solely for research and analysis purposes into the Windows PE file format.  If you aren't here for that reason and ONLY that reason, then this repository is not legal for you to use.

[![Donate](https://cubiclesoft.com/res/donate-shield.png)](https://cubiclesoft.com/donate/) [![Discord](https://img.shields.io/discord/777282089980526602?label=chat&logo=discord)](https://cubiclesoft.com/product-support/github/)

Features
--------

* 375+ real-world PE file format binary artifacts in a single repo.
* Spans decades of computing and a wide range of criteria but only occupies about 64MB of disk storage.  Some artifacts are as small as 2KB!
* Large selection of both 32-bit and 64-bit Windows PE file samples.
* Some DOS MZ and Win16 NE samples too.
* Detailed origin information for each artifact.
* Malware free.
* Probably the largest, most complete, organized, and succinct public library of unique PE artifact samples in the world.  Great for building and validating PE file format software libraries!
* Files are organized by each possible option within each PE file format structure as defined by the Microsoft Windows PE/COFF specification.
* Sits on GitHub for all of that issue tracker goodness to easily submit changes and ideas respectively.

Copyright Notes
---------------

As a user, you may only CLONE, DOWNLOAD, star, and/or follow this repository.  However, republishing this repository and/or its contents carries significant legal risks.  When republishing this repo, you will incur all legal responsibilites associated with the repository and therefore republishing this repo may be illegal depending on where in the world you live.

GitHub forks may be considered in some jurisdictions as republishing despite the fact an unmodified fork is just a pointer to a specific commit in another repository (i.e. it's just a link).  To be on the safe side though, do not fork this repository.  The usual purpose of a fork is to modify it (aka a modified fork) and then open a pull request.  Out of an abundance of caution, pull requests against this repo will be rejected for this reason.  See "Submitting New Samples" below.

When used solely as intended for research and analysis purposes of the PE file format, this repository, its contents, and its users are protected under the narrowly defined Fair Use clauses of U.S. Copyright Law.  Most of the artifacts in this repo are randomly selected files that just happened to meet certain criteria during automated system scans and were included as a result but are generally useless without their supporting software.  That clever little PE file format trick your developers used years ago is the most likely reason why it shows up here now.  If you are the copyright holder of a binary found in this repo, please open an issue on the issue tracker or contact CubicleSoft directly with any questions.  Intentional software piracy is not condoned by CubicleSoft or its partners.  At the discretion of CubicleSoft, binaries may be replaced, removed, or code-neutralized in response to the valid request of a copyright holder.

Submitting New Samples
----------------------

To submit a new sample:

* Submissions without proper spelling or punctuation when describing details about a sample will be summarily rejected.  Also, be professional and use language suitable for polite company.
* Use the `pe_tools.php artifacts origins` option to generate the correct text files for sample submissions.  All fields are required.
* Must not contain malware.  While some of the more interesting PE samples out there are found in the malware universe, this repo is for standard PE files only.
* Submitted samples must either be:  Unique in some way not seen before (`pe_tools.php artifacts find` will report rarity) OR be significantly smaller than the existing sample.
* Pull requests depend on forking, which, as previously mentioned under Copyright Notes, are disallowed for legal reasons.  Submissions of samples must be made via file upload to the issue tracker.  The GitHub issue tracker allows both ZIP and .tar.gz files.

Other PE Artifact Libraries
---------------------------

* https://github.com/corkami/pocs/tree/master/PE

The above artifacts have NOT been vetted by CubicleSoft.  Be careful when handling unknown executables.  Your mileage may vary in terms of legitimacy, quality, and safety.
