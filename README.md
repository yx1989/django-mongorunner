# Django Mongorunner

A testrunner for django using mongodb with mongoenngine.

## Install

Simply specify mongorunner as your testrunner in settings.py:
    TEST_RUNNER = 'mongorunner.TestRunner'

## Usage

    from mongorunner import TestCase

    class SimpleTest(TestCase):
        def test(self):
            pass

## Attection

This runnser only can use in django1.4, maybe can use in django1.5, but can't use in django1.6. Because of django changed it's TransactionTestCase in v1.6.

Also need pay attection to DiscoverRunner if you want auto find testcases.
