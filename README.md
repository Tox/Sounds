Introduction
============

This repository hosts a collection of FLAC-encoded sounds that Tox client
developers may pick up and use freely in their software.

Contributing
============

At the top level, the repository is organized by the name of the sound pack.
Underneath that, the repository is organized into categories of sounds, where
each sound is named according to its purpose (See the "File Naming" and "Sound
Descriptions" sections below). Submitted sound collections **must** be
formatted according to this naming scheme and folder structure, so that clients
are easily able to plug in different sound collections.

To contribute, just submit a pull request containing your FLAC-encoded sounds.
Your work must be released under a **free** license in order to be included in
this repository, and this license must be included in the top level of your
respective sound collections.

File Naming
===========

Submitted sound packs must match the following file heirarchy and naming
scheme.

    =Ringtone
        |-IncomingVideo.flac
        |-IncomingAudio.flac
        |-OutgoingVideo.flac
        |-OutgoingAudio.flac
    =Notification
        |-CallDrop.flac
        |-GeneralError.flac
        |-ContactOffline.flac
        |-ContactOnline.flac
        |-Invite.flac
        |-Message.flac
        |-ImportantMessage.flac
        =FileTransfer
            |-Failure.flac
            |-Incoming.flac
            |-Resume.flac
            |-Success.flac
        =Group
            |-Leave.flac
            |-NameChange.flac
            |-Join.flac

Sound Descriptions
==================

This section gives descriptions of the use-case for each sound, and (when
relevant) an example of what could constitute that use-case. However keep in
mind that clients are free to choose how these sounds are used, and there's no
guarantee that what one client calls an "Important Message" is the same as
another client's definition.

## Ringtone

Sound         | Description
------------- | -----------------------------------------------------
IncomingVideo | The client is receiving a video call from a contact.
IncomingAudio | The client is receiving an audio call from a contact.
OutgoingVideo | The client is making a video call to a contact.
OutgoingAudio | The client is making an audio call to a contact.

## Notification

Sound            | Description                       | Example
---------------- | --------------------------------- | -------------------------------------------------------------------
CallDrop         | A call has ended unexpectedly.    | Toxcore has just timed out in the middle of an audio or video call.
GeneralError     | An error has occurred.            | The client was unable to save a file to disk.
ContactOnline    | The client has connected to a contact who was previously offline. | 
Invite           | The client has received a friend request or group join request. | 
Message          | The client has received a message from a contact. | 
ImportantMessage | The client has received an important message | The client has received a hilight message in a groupchat; the message includes the user's name.

### FileTransfer

Sound    | Description
-------- | -----------------------------------------------------------------
Failure  | A file transfer has failed.
Incoming | The client is receiving a file transfer request from a contact.
Resume   | The client is resuming a file transfer that was previously paused.
Success  | The client has successfully completed a file transfer.

### Group

Sound      | Description
---------- | -----------------------------------------------------
Leave      | The client has left a groupchat that it was joined to.
NameChange | A peer joined to the same groupchat as the client has changed their display name.
Join       | The client has joined a groupchat to which it was not previously joined.


If you have any suggestions for new sound types, feel free to open a pull
request or file an issue.

Thanks, and happy sound...ing
