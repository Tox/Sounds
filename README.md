Introduction
============

This repository hosts a collection of sounds that Tox client developers may
pick up and use freely in their software.

Contributing
============

At the top level, the repository is organized by the name of the "sound pack",
or whatever it is that you'd like to call your collection of sounds.
Underneath the top level, the repository is organized into categories of
sounds, where each sound is named according to its purpose (See the "File
Naming" section below). Submitted sound collections **must** be formatted
according to this naming scheme and folder structure, so that clients are
easily able to plug in different sound collections.

To contribute, just submit a pull request containing your sounds in a lossless
format. Your work must be released under a **free** license in order to be
included in this repository, and this license must be included in the top level
of your respective sound collections.

File Naming
===========

Your sound files should be named according to the following list of standard
file names.

    =Ringtone
        |-IncomingVideo.ext
        |-IncomingAudio.ext
        |-OutgoingVideo.ext
        |-OutgoingAudio.ext
    =Notification
        |-CallDrop.ext
        |-GeneralError.ext
        |-ContactOffline.ext
        |-ContactOnline.ext
        |-Invite.ext
        |-Message.ext
        |-ImportantMessage.ext
        =FileTransfer
            |-Failure.ext
            |-Incoming.ext
            |-Resume.ext
            |-Success.ext
        =Group
            |-Leave.ext
            |-NameChange.ext
            |-Join.ext

    Key:
    = - Folder
    .ext - The file extension appropriate for your losslessly-encoded media
    (FLAC, WAV, etc.)

If you have any suggestions for new sound types, feel free to open a pull
request or file an issue.

Thanks, and happy sound...ing
