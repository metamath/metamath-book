# Errata

The following are errata for the Metamath 2019 ("Second Edition") book
dated 2019-06-02:

* Preface (Note Added March 7, 2019) - Matamath --> Metamath
* Section 1.4.2 (page 32, paragraph 3) -
  there's an extraneous ")" after the term set.mm.
* Section 2.4 (page 52) and further shows this text after some assign commands:
  "To undo the assignment, DELETE STEP ... and INITIALIZE, UNIFY if needed."
  This text is no longer shown.
  When the first edition of the book was written, metamath.exe didn't have
  the 'undo'/'redo' commands (added in 2013; see 'help undo'), so hints
  were provided by some commands for how to undo them manually.
  These hints are no longer displayed since they are no longer needed.
* Section 3.3.2 and 3.3.3 headings (page 71) - the headings go past
  the intended margin (though they're quite readable).
* Section 3.9.3 (page 97) - "appraoch" should be "approach".
* Section 4.3 (page 138) - there is a superfluous comma:
  "... option to hide, them, but today ...".
* Section 4.3.1 (page 139) - "used and that each $f hypothesis have"
  should be "used, and each $f hypothesis must have".
* Section 4.5.4 (page 155) - "Metmath" should be "Metamath".
* Chapter 5 mentions the minimize command, but does not describe it
  in detail. A future version of the book might describe it in more detail.
* Section 5.6.3 `set empty_substitution` Command (page 171) -
  there's a duplication and the first bracketed text could be removed.
  It says:
  "(An example where this must be on would
  be a system that implements a Deduction Rule and in which deductions from
  empty assumption lists would be permissible. The MIU-system described in
  Appendix D is another example.) Note that empty substitutions are always
  permissible in proof verification (VERIFY PROOF...) outside the Proof
  Assistant. (See the MIU system in the Metamath book for an example of
  a system needing empty substitutions; another example would be a system
  that implements a Deduction Rule and in which deductions from empty
  assumption lists would be permissible.)"

