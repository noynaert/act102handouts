# Bootstrap 020 

# Alpha, Beta, RC, Stable, LTS

By this point in the semester you probably understand something about how easy it is to let little glitches into your software, especially as that software gets more complex.

There is a system for releasing software.  Typically software goes through an "Alpha-Beta-Stable-Release Life Cycle."

Alpha and Beta are considered test candidates.  Products that contain Alpha and Beta level code should not be used in commercial or final projects.

## Alpha 

Alpha level code is assumed to have serious bugs.  Using it could cause crashes and data loss.  It is also possible some features are not fully functional.

For the most part inexperienced users should stay away from Alpha level code.

Sometimes there are different Alpha versions.  These are typically numbered as Alpha1 and Alpha2

It used to be that Alpha code was never released publicly.  It would be tested internally by the developer.  Late in the Alpha stage it might be released to some large and experienced users who could test it in their own environments.  It is now fairly common for late-stage alpha code to be released publicly.

## Beta

Beta code has all the features as complete and without major errors.

Beta code sometimes is divided into "Private Beta" and "Public Beta."  Private Beta is generally distributed to people who have experience with previous versions of the product.  Sometimes beta software is open to everyone, but you have to do something like join the developer network to get access to it.

The company will not provide regular technical support for the product, but it will usually have a mechanism for reporting bugs.

### Release Candidate

RC is effectively a late version of Beta.  The developers think it is ready to go, but they want final testing.  Sometimes they just want to test that the install methods for the final product are working properly.  It is also used to help train the technical support staff.

## Stable

Stable releases should be ready for public use.  There should be no significant bugs.  All the features should be working as advertised.  Generally the developer will supply technical support.

## LTS

LTS is actually a stage beyond Stable.  Sometimes developers will release software as "Long Term Support."  

The company promises to provide updates and fixes for a longer period of time than for regular releases.  

* There typically are not a lot of new features
* There is typically a longer and more careful beta testing phase

An example is Ubuntu Linux.  Ubuntu releases .  LTS versions are released in April of even-numbered years.  They are supported for five years instead of one.  In fact, if you are a customer of Ubuntu you can get security updates for 10 years.

## What version should you use?

If you are working on a team, it is important that all members of the team work on the same version.  If software is going to be released for public use, it should be done with the latests stable version.  Sometimes a business will have a standard that is an older model.  They are willing to forgo some of the later features to stay with a version that they are familiar with and that works for them.

If you get to chose a version, then it is usually best to pick the latest stable version. 

Sometimes developers will use a late-beta or RC version because they expect the stable version to be released before their product is released, but this can be risky.

Commercial products that are in actual use should be at least using stable version.  They should use LTS versions if they are available.