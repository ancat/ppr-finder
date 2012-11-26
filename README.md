ppr-finder
==========

A WinDbg script to find pop-pop-ret sequences within a module loaded in memory.

Goes great with narly!

Basic Instructions
==================

How to use ppr-finder with narly:

    1. Load narly
    2. Enumerate target modules with !nmod
    3. Pick an address range belonging to a module, preferably without ASLR and SafeSEH off
    4. Run the script
        $$>a<c:\ppr-finder.wds 0xSTART 0xEND
    5. Pick any address