# CBT368
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. GitHub repos will be deleted and created during this period...

```
//***FILE 368 is from James Williams of Atlanta, Georgia, and       *   FILE 368
//*           contains a collection of his tools and utilities.     *   FILE 368
//*                                                                 *   FILE 368
//*      email:  "James Williams" <jwilliam@aglresources.com>       *   FILE 368
//*                                                                 *   FILE 368
//*                 James Williams                                  *   FILE 368
//*                 AGL Resources (Services) Co.                    *   FILE 368
//*                 1219 Caroline Street                            *   FILE 368
//*                 Atlanta, GA 30307                               *   FILE 368
//*                 404-584-4112                                    *   FILE 368
//*                                                                 *   FILE 368
//*      Here is a short description of the contents of this        *   FILE 368
//*      file:                                                      *   FILE 368
//*                                                                 *   FILE 368
//*      ALL REXX SMF STUFF MUST BE RECFM=VB INSTEAD OF             *   FILE 368
//*      RECFM=VBS AS REXX CANNOT HANDLE SPANNED RECORDS.           *   FILE 368
//*                                                                 *   FILE 368
//*      $$$DOC   - This member                                     *   FILE 368
//*                                                                 *   FILE 368
//*      AL       - Good when you are at 3.4 and need to            *   FILE 368
//*                 duplicate a dataset                             *   FILE 368
//*                                                                 *   FILE 368
//*      COMMAND  - Added support for 4 digit reply id to           *   FILE 368
//*                 program from File 019 issue 'FIND *JAW*' to     *   FILE 368
//*                 see my changes.                                 *   FILE 368
//*                                                                 *   FILE 368
//*      COPYLNES - Great taking a dataset file and then create     *   FILE 368
//*                 a record before each.  This is great for        *   FILE 368
//*                 creating multi-line control cards               *   FILE 368
//*                                                                 *   FILE 368
//*      DMPGENER - This simple REXX takes a dataset list and       *   FILE 368
//*                 generates control cards for DFDSS.  I use       *   FILE 368
//*                 this same example to create JCL and other       *   FILE 368
//*                 control card schemes.                           *   FILE 368
//*                                                                 *   FILE 368
//*      FTAILSMF - FTAILSMF is BAL program that shows the power    *   FILE 368
//*                 of ISPF calls. You can easily manage datasets   *   FILE 368
//*                 using ISPF calls which do the SVC 99 stuff      *   FILE 368
//*                 under the doors. Also, a REXX version in there. *   FILE 368
//*                                                                 *   FILE 368
//*      IEFUJI   - IEFUJI exit to gets info from ACF2.  Probably   *   FILE 368
//*                 would not take much to get from RACF or Top     *   FILE 368
//*                 Secret also.  Also creates an SMF record        *   FILE 368
//*                 (128) processed by SMF128J.                     *   FILE 368
//*                                                                 *   FILE 368
//*      JOBID    - Simple REXX to find JOBID                       *   FILE 368
//*                                                                 *   FILE 368
//*      MSGCHECK - Little REXX program to check MPF.  IEAVMXIT     *   FILE 368
//*                 must be active for some AUTOOPS packages.       *   FILE 368
//*                                                                 *   FILE 368
//*      RDATE    - REXX date routine. Recently added some Y2K      *   FILE 368
//*                 updates.  REXX date function has most of this   *   FILE 368
//*                 support today.  Originally a CLIST from CBT,    *   FILE 368
//*                 I believe, that I converted to REXX and         *   FILE 368
//*                 updated.                                        *   FILE 368
//*                                                                 *   FILE 368
//*      RXJOBID  - Assembler REXX function same as JOBID above.    *   FILE 368
//*                 Shows how simple BAL REXX functions are.        *   FILE 368
//*                                                                 *   FILE 368
//*      SEQNUM   - Handy member.  I once had a job with a          *   FILE 368
//*                 zillion steps all with the same name.  This     *   FILE 368
//*                 edit macro made each step unique.               *   FILE 368
//*                                                                 *   FILE 368
//*      SMF128   - For poor shops without SAS, REXX is a great     *   FILE 368
//*                 tool for quick SMF data reports for auditors    *   FILE 368
//*                 or bean counters.                               *   FILE 368
//*                                                                 *   FILE 368
//*      SMF128J  - JCL to invoke SMF128 user SMF record from       *   FILE 368
//*                 IEFUJI.                                         *   FILE 368
//*                                                                 *   FILE 368
//*      SMF170   - For poor shops without SAS, REXX is a great     *   FILE 368
//*                 tool for quick SMF data reports for auditors    *   FILE 368
//*                 or bean counters. SMF170 records from FILEAID   *   FILE 368
//*                 require an AUTHSVC.                             *   FILE 368
//*                                                                 *   FILE 368
//*      SMF170J  - JCL to invoke SMF170 to report on               *   FILE 368
//*                 FILEAID edits.                                  *   FILE 368
//*                                                                 *   FILE 368
//*      PCOPY    - This edit macro extends the power of the        *   FILE 368
//*                 COPY command.  PCOPY can copy a PROC member     *   FILE 368
//*                 without the intervening copy panel.  I need     *   FILE 368
//*                 to expand this for non-pds's also.              *   FILE 368
//*                                                                 *   FILE 368
//*      COBPRT   - Simple program to test our Y2K date             *   FILE 368
//*                 simulator.  This executes COBOL II date         *   FILE 368
//*                 calls.  COBOL for MVS has some examples in      *   FILE 368
//*                 the IVP.                                        *   FILE 368
//*                                                                 *   FILE 368
//*      PLIAVG   - Simple program to test our Y2K date             *   FILE 368
//*                 simulator.  This executes PLI date calls at     *   FILE 368
//*                 the 2.3 level.                                  *   FILE 368
//*                                                                 *   FILE 368
//*      STCK     - Simple program to test our Y2K date             *   FILE 368
//*                 simulator.  This executes a STCK instruction.   *   FILE 368
//*                                                                 *   FILE 368
//*      TIMEPC   - Simple program to test our Y2K date             *   FILE 368
//*                 simulator.  This executes a TIME PC call.       *   FILE 368
//*                                                                 *   FILE 368
//*      TIMEX    - Simple program to test our Y2K date             *   FILE 368
//*                 simulator.  This executes a regular TIME        *   FILE 368
//*                 call.                                           *   FILE 368
//*                                                                 *   FILE 368
//*      TOUPPERC - Xpediter will not handle lower case             *   FILE 368
//*                 code as of 10-06-1999. Converts all text        *   FILE 368
//*                 to uppercase prior to assembly.                 *   FILE 368
//*                                                                 *   FILE 368
//*      TOUPPERJ - Job to run invoke TOUPPERC against your         *   FILE 368
//*                 PDS. It uses STARTOOL or PDS85 to invoke.       *   FILE 368
//*                 Good control card examples.                     *   FILE 368
//*                                                                 *   FILE 368
//*      WTOAGL01 - Example of a TSO exit to start all VTAM         *   FILE 368
//*                 appls at our site.  Would require a IST020I     *   FILE 368
//*                 entry to start this exit in MPFLST00.  The      *   FILE 368
//*                 last byte of each of our SMF ids is unique,     *   FILE 368
//*                 such as SYSA, SYSB, or SYSC.  It grabs the      *   FILE 368
//*                 character, as we have unique requirements for   *   FILE 368
//*                 each system.                                    *   FILE 368
//*                                                                 *   FILE 368
```
