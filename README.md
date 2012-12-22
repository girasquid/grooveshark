Grooveshark
====

This is a simple wrapper for the Grooveshark API.

Usage
====

    from grooveshark.client import Grooveshark
    client = Grooveshark('key', 'secret')
    print client.call('pingService')
    client.authenticate('username', 'password') # returns True if username/password is good; raises GroovesharkException if not
    print client.call('getUserPlaylists')