Description:
This test file includes unit tests for the Barky bookmarking application

Dependencies:
This test file requires the Barky bookmarking application to be installed

Instructions:
To run the tests, navigate to the directory containing the test file and run python -m unittest

Results:
Each test checks a different application functionality, such as adding bookmarks, deleting bookmarks, and searching for bookmarks. All tests should pass if the application is functioning correctly. Such as:

test_add_bookmark: Tests that a bookmark can be added to the database and the number of bookmarks increases by 1.
test_delete_bookmark: Tests that a bookmark can be deleted from the database and the number of bookmarks decreases by 1.
test_edit_bookmark: Tests that a bookmark's title can be updated in the database.
test_list_bookmarks: Tests that all bookmarks in the database can be listed and the correct number of bookmarks are returned.
test_search_bookmarks: Tests that bookmarks containing a given search term are returned.
test_add_duplicate_bookmark: Tests that try to add a bookmark already existing in the database raise an exception.
test_list_bookmarks_empty and test_search_bookmarks_empty: Tests check that the list and search functions return an empty list when there are no bookmarks in the database.

test_edit_nonexistent_bookmark and test_delete_nonexistent_bookmark: Tests check that the edit and delete functions raise a Bookmark.DoesNotExist exception when attempting to edit or delete a bookmark that does not exist in the database.

Edge Cases
Edge cases are cases that are less common or less expected than the typical behavior of the application. Adding these extra test cases helps ensure that the Barky app is functioning properly in these edge cases as well.

These are a few examples of edge cases that are tested here:

Adding a duplicate bookmark
Attempting to edit a nonexistent bookmark
Attempting to delete a nonexistent bookmark
Listing bookmarks when there are no bookmarks in the database
Searching for bookmarks when there are no bookmarks in the database

