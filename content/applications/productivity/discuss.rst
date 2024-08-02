:show-content:
:hide-page-toc:

=======
Discuss
=======

Odoo **Discuss** is an internal communication app that allows users to connect through messages,
notes, file sharing, and video calls. **Discuss** enables communication through a persistent chat
window that works across applications, or through the dedicated **Discuss** dashboard.

Inbox, starred, and history
===========================

On the :guilabel:`Discuss` dashboard, unread messages are visible in the :guilabel:`Inbox`.
:guilabel:`Starred` is where starred messages are stored. :guilabel:`History` shows *Chatter*
updates for records in the Odoo database that the user has been assigned to, or tagged on.

Direct messages
===============

*Direct messages* allow the user to communicate privately with one or multiple team members. To
start a new direct message, click the :icon:`fa-plus` icon next to :guilabel:`Direct Messages` on
the :guilabel:`Discuss` dashboard, and enter the name of the desired person in the search bar that
appears.

Direct message actions
----------------------

Hover over a direct message in the chat window to see a menu of actions to take on the message.

.. image:: discuss/direct-message-actions.png
   :alt: View direct message actions.

Click :icon:`fa-smile-o` :guilabel:`Add a Reaction` to open a drop-down menu of emojis that can be
used to react to the direct message. Click :icon:`fa-reply` :guilabel:`Reply` to reply to the direct
message in a thread. Click :icon:`fa-star-o` :guilabel:`Mark as Todo` to add the message to the
:guilabel:`Starred` tab. Clicking :icon:`fa-ellipsis-h` :guilabel:`Expand` reveals more message
actions, including :icon:`fa-thumb-tack` :guilabel:`Pin`, :icon:`fa-eye-slash` :guilabel:`Mark as
Unread`, :icon:`fa-pencil` :guilabel:`Edit`, and :icon:`fa-trash` :guilabel:`Delete`.

Conversation actions
--------------------

The icons in the top-right corner of a direct message conversation represent different actions the
user can take on that conversation.

.. image:: discuss/conversation-actions.png
   :alt: View of the conversation actions.

Click :icon:`fa-bell` :guilabel:`Notification Settings` to set up notification preferences for the
conversation, or click :icon:`fa-phone` :guilabel:`Start a Call` to begin a meeting. See the
:ref:`Meetings <discuss/meetings>` section for more information about meetings.

Click :icon:`fa-search` :guilabel:`Search Messages` to search messages in the conversation.

Clicking :icon:`fa-thumb-tack` :guilabel:`Pinned Messages` shows pinned messages, and clicking
:icon:`fa-paperclip` :guilabel:`Show Attachments` shows attachments shared in the conversation.

Click :icon:`fa-user-plus` :guilabel:`Add Users` to invite more people to the direct message
conversation. Click :icon:`fa-cog` :guilabel:`Show Call Settings` to configure voice chat settings.

At the top of the direct message window, click the name of the direct message to change the group
name, and choose to add a description in the adjacent :guilabel:`Add a description` field.

User status
-----------

It is helpful to see what colleagues are up to, and how quickly they can respond to messages by
checking their *status*. The status is shown on the right side of a contact's name on the sidebar,
on the *messaging menu*, and when listed in the *Chatter*.

- Green = online
- Orange = away
- White = offline
- Airplane = out of the office

Delete a direct message conversation
------------------------------------

To delete direct message conversations, click the :guilabel:`X` next to the name in the
:guilabel:`Direct Messages` section of the sidebar.

.. note::
  This does **not** delete the :guilabel:`Direct Messages` in the conversation. The direct message
  conversation's history is visible when another direct message with the same person, or group, is
  created.

.. _discuss/meetings:

Meetings
========

In **Discuss**, :guilabel:`Meetings` are video calls. To start a meeting from the **Discuss**
application home page, click :guilabel:`Start a meeting` in the top-left corner, and select who to
invite to the meeting, via the :guilabel:`Invite People` drop-down window that appears. To start a
meeting from a direct message, click the :icon:`fa-phone` :guilabel:`Start a Call` icon in the
top-right.

.. image:: discuss/meeting.png
   :alt: View of a Meeting in Odoo Discuss.

Once a meeting has been started, the buttons on the bottom of the call screen can be used to
:icon:`fa-microphone` :guilabel:`Mute/Unmute`, :icon:`fa-headphones` :guilabel:`Deafen/Undeafen`,
and :icon:`fa-video-camera` :guilabel:`Turn camera on/off`. Clicking the :icon:`fa-ellipsis-v`
:guilabel:`More` icon allows the user to :icon:`fa-hand-paper-o` :guilabel:`Raise Hand`,
:icon:`fa-desktop` :guilabel:`Share Screen`, or :icon:`fa-arrows-alt` :guilabel:`Enter Full Screen`.

Configuration
=============

Selecting :guilabel:`Configuration` at the top of the Discuss homepage triggers a drop-down menu of
options including :guilabel:`Notification` :guilabel:`Voice & Video`, and :guilabel:`Canned
Responses`.

Select :menuselection:`Configuration --> Notification` to mute a server or adjust the channel's
notification settings.

Select :menuselection:`Configuration --> Voice & Video` to select a voice input device, select
:guilabel:`Voice Detection` or :guilabel:`Push to Talk`, set the voice detection threshold, and
toggle :guilabel:`Show video participants only` and :guilabel:`Blur video background`.

Select :menuselection:`Configuration --> Canned Responses` to configure canned responses.

.. _discuss_app/notification_preferences:

Choose notifications preference
===============================

Access user-specific preferences for the *Discuss* app by navigating to :menuselection:`Settings app
--> Manage Users`, select a user, and then click the :menuselection:`Preferences` tab.

.. image:: discuss/preferences-user.png
   :alt: View of the Preferences tab for Odoo Discuss.

By default, the :guilabel:`Notification` field is set as :guilabel:`Handle by Emails`. With this
setting enabled, a notification email is sent by Odoo every time a message is sent from the
chatter, a note is sent with an `@` mention (from *Chatter*), or a notification is sent for a record
that the user follows. Something that triggers a notification is changing of the stage (if an email
is configured to be sent, for example if the task is set to :guilabel:`Done`).

By choosing :guilabel:`Handle in Odoo`, the above notifications are shown in the *Discuss* app's
:guilabel:`Inbox`.

Chat from different applications
================================

The *Discuss* application enables communication across all of Odoo's applications. To view chats and
channels, or start a new message, select the speech bubbles in the upper right corner of another app
in Odoo.

.. image:: discuss/discuss-in-other-apps.png
   :alt: Use Discuss across other applications by clicking the speech bubbles.

.. seealso::
   - :doc:`discuss/team_communication`
   - :doc:`/applications/essentials/activities`
   - :doc:`discuss/ice_servers`
   - :doc:`discuss/chatter`

.. toctree::
   :titlesonly:

   discuss/team_communication
   discuss/ice_servers
   discuss/chatter
