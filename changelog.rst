=========
Changelog
=========

v0.8.0b1
--------

Server:

- New query2 API for querying and transforming data
- Added :code:`version` field to :code:`/info` endpoint
- Set stricter allowed CORS origins in testing mode
- Added :code:`--cors-origins` CLI argument

Web UI:

- Added datepicker to the activity view
- Moved the today/clock visualization into the activity view
- New visualization for most-visited domains
- New visualization for previous days active time
- New query explorer
- Now displays version and hostname in bottom-right corner
- Now uses aw-client-js for all API calls

Watchers:

- Improved stability of client event queues (`see this PR <https://github.com/ActivityWatch/aw-client/pull/28>`_)

Other:

- Windows: Console window and taskbar icon now hidden by default (`issue #139 <https://github.com/ActivityWatch/activitywatch/issues/139>`_)
- All issues assigned to the v0.8 milestone can be found `on GitHub <https://github.com/ActivityWatch/activitywatch/milestone/1>`_

v0.7.1
--------

- Actually fixed the timezone issue in the web UI (`issue #117 <https://github.com/ActivityWatch/activitywatch/issues/117>`_).
- All issues assigned to the v0.7 milestone can be found `on GitHub <https://github.com/ActivityWatch/activitywatch/milestone/4>`_.

v0.7.0b4
--------

- The ActivityWatch WebExtension is now supported from this version forward, see the announcement `on the forum <https://forum.activitywatch.net/t/you-can-now-track-your-web-browsing-with-activitywatch/28>`_.
- (Not really, see v0.7.1) Fixed pesky timezone issue in web UI (`issue #117 <https://github.com/ActivityWatch/activitywatch/issues/117>`_).
- Fixed bug on macOS where keyboard activity would not be used to detect AFK state.
- Fixed packaging bugs (macOS, PyInstaller).
- The web extension now has a better look and notifies if connection to server failed.

v0.7.0b3
--------

- Even more improvements to the web UI.
- Major improvements to the documentation, notably instructions on how to install from builds and sources.

v0.7.0b2
--------

- Improvements to the web UI: a new visualization method (the "today" view) and information for users about the state of the project on the first page.

v0.7.0b1
--------

There have been several major changes since v0.6. Much of it wont end up here but hopefully the major things will.

.. note::
    If you are upgrading from a previous version, you might want to stop all loggers for the duration of your UTC offset to prevent issues which we've had difficulty debugging (or you can just start right away and expect your first hours to end up a bit weird).

- Now works on Windows.
- Working standalone packages. (edit: not reliable on all systems, but a lot easier to get running in many cases)
- All timestamps are now in UTC.
- Updated outdated parts of the documentation.
- Makefiles are now used throughout the projects to manage building, testing, and CI.
- A lot of bug fixes (and hopefully not too many new bugs).
- Vastly improved code quality.

v0.6.0 and older
----------------

We haven't been keeping track of changes very well for older versions. Please refer to the git history.
