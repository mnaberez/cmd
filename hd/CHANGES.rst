2015-12-09
----------

- ``SET HD CLOCK``: Added an ``IF`` statement to end of line 30 to fix a
  crash.  After the RTC battery was replaced in a CMD HD, the day of week
  returned a nonsensical value (variable ``WD``) that was out of bounds
  of the ``WD$()`` array, which caused ``?BAD SUBSCRIPT ERROR IN 1100``.
