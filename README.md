
# Atributes


#### Setting passwords for the Lumenvox

You can set passwords via attributes

    node['lumenvox']['client']['authentication_username']  =  foo
    node['lumenvox']['client']['authentication_password']  =  foo

Or you can pass then in via environment prior to running Chef

    export LUMENVOX_USERNAME=foo
    export LUMENVOX_PASSWORD=bar
    chef-solo -c solo.rb -j dna.json -l debug


Setting versions

    {
        "lumenvox": {
            "sre": {
                "version": "10.5.300-1.el5"
            },
            "core": {
                "version": "10.5.300-1.el5"
            },
            "license_server": {
                "version": "10.5.300-1.el5"
            },
            "media_server": {
                "version": "10.5.300-1.el5"
            },
            "client": {
                "version": "10.5.300-1.el5"
            },
            "tts": {
                "version": "10.5.300-2SF.el5",
                "voices": [
                    {
                        "voice": "Jason",
                        "version": "10.5.110-1"
                    }
                ]
            }
        }
    }
