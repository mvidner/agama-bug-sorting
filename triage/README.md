# triage script

Usage: triage https://bugzilla.suse.com/show_bug.cgi?id=9999999

- extracts the bug number ($BUGNUM) from the URL
- makes a ~/bugs/$BUGNUM directory
- asks the user for a terse bug title
- symlinks ~/bugs/$BUGNUM-terse-bug-title -> $BUGNUM
