git-describe - Give an object a human readable name based on an available ref
DESCRIPTION
The command finds the most recent tag that is reachable from a commit. If the tag points to the commit, then only the tag is shown. Otherwise, it suffixes the tag name with the number of additional commits on top of the tagged object and the abbreviated object name of the most recent commit. The result is a "human-readable" object name which can also be used to identify the commit to other git commands.

By default (without --all or --tags) git describe only shows annotated tags. For more information about creating annotated tags see the -a and -s options to git-tag[1].

If the given object refers to a blob, it will be described as <commit-ish>:<path>, such that the blob can be found at <path> in the <commit-ish>, which itself describes the first commit in which this blob occurs in a reverse revision walk from HEAD.
