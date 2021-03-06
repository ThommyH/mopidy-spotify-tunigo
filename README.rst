*********************
Mopidy-Spotify-Tunigo
*********************

.. image:: https://img.shields.io/pypi/v/Mopidy-Spotify-Tunigo.svg?style=flat
    :target: https://pypi.python.org/pypi/Mopidy-Spotify-Tunigo/
    :alt: Latest PyPI version

.. image:: https://img.shields.io/pypi/dm/Mopidy-Spotify-Tunigo.svg?style=flat
    :target: https://pypi.python.org/pypi/Mopidy-Spotify-Tunigo/
    :alt: Number of PyPI downloads

.. image:: https://img.shields.io/travis/trygveaa/mopidy-spotify-tunigo/master.png?style=flat
    :target: https://travis-ci.org/trygveaa/mopidy-spotify-tunigo
    :alt: Travis CI build status

.. image:: https://img.shields.io/coveralls/trygveaa/mopidy-spotify-tunigo/master.svg?style=flat
   :target: https://coveralls.io/r/trygveaa/mopidy-spotify-tunigo?branch=master
   :alt: Test coverage

`Mopidy <http://www.mopidy.com/>`_ extension for providing the browse feature
of `Spotify <http://www.spotify.com/>`_. This lets you browse playlists, genres
and new releases.

Uses the `Tunigo <http://tunigo.com/>`_ API, which is also what Spotify itself
uses. Note that the API is not documented or officially released, so it may
change at any time.


Dependencies
============

- ``Mopidy`` >= 0.19.0. The music server that Mopidy-Spotify-Tunigo extends.

- ``Mopidy-Spotify`` >= 1.2.0. The Mopidy extension for playing music from
  Spotify.

- ``Python-Tunigo``. A library for accessing the Tunigo API.


Installation
============

Debian/Ubuntu/Raspbian: Install the ``mopidy-spotify-tunigo`` package from
`apt.mopidy.com <http://apt.mopidy.com/>`_::

    sudo apt-get install mopidy-spotify-tunigo

Arch Linux: Install the ``mopidy-spotify-tunigo`` package from
`AUR <https://aur.archlinux.org/packages/mopidy-spotify/>`_, e.g.::

    yaourt -S mopidy-spotify-tunigo

Else: Install the ``Mopidy-Spotify-Tunigo`` package from PyPI::

    pip install Mopidy-Spotify-Tunigo


Configuration
=============

The following configuration values are available:

- ``spotify_tunigo/enabled``: If the Spotify-Tunigo extension should be enabled
  or not.
- ``spotify_tunigo/region``: The region to fetch playlists and releases for.
  Either "all" or a two letter country code. Defaults to "all".
- ``spotify_tunigo/cache_time``: The amount of seconds to cache the results
  from the API. A value of 0 will disable the cache. Defaults to 3600.


Project resources
=================

- `Source code <https://github.com/trygveaa/mopidy-spotify-tunigo>`_
- `Issue tracker <https://github.com/trygveaa/mopidy-spotify-tunigo/issues>`_
- `Download development snapshot <https://github.com/trygveaa/mopidy-spotify-tunigo/archive/master.tar.gz#egg=Mopidy-Spotify-Tunigo-dev>`_


Changelog
=========

v0.2.1 (2014-07-21)
-------------------

- Update dependencies
- Fix flake8 errors, unused imports and docs syntax
- Test config options

v0.2.0 (2014-06-23)
-------------------

- Move Tunigo API into a separate library
- Add option to specify cache time
- List top tracks and sub genres in each genre

v0.1.0 (2014-06-21)
-------------------

- Initial release.
