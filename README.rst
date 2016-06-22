===============
GIT - PHP check
===============

:Author: Remigijus Jarmalavicius <remigijus(a)jarmalavicius.lt>
:Thanks to: Vytautas Povilaitis <php-checker(a)vytux.lt>
:Thanks to: hkdobrev (https://github.com/hkdobrev)
:Thanks to: Cliff Seal (https://github.com/logoscreative)
:Thanks to: Dave Barnwell (https://github.com/freshsauce)

About
-----
GIT hook for PHP parse errors checking before commit.

If you looking same thing for Mercurial DCVS, check this out:

    http://www.bitbucket.org/vytux/mercurial-plugin-4-syntax-checking

How to install
--------------
To install hook, copy pre-commit file to your project .git/hooks/pre-commit:

    $ cp pre-commit .git/hooks/pre-commit;
    $ chmod +x .git/hooks/pre-commit;

Now, when you will make some modifications for code and will try to commit, GIT
will stop you and tells where problem exist.

Usage example
-------------

Example of PHP script beeing commited with PHP syntax errors:

    Syntax errors found in file: cms/content.php 

    Found PHP parse errors: 
    PHP Parse error: syntax error, unexpected ')' in /path/to/project/cms/content.php on line 39

    Fix errors and commit again.


Config
------
    linter.php.silent : (type: boolean) Suppresses all messages that are not linter errors.

Bugs
----
If you have found any bugs, please track them here:

    https://github.com/ReekenX/git-php-syntax-checker/issues

Thanks for all peoples who made this tool better.
