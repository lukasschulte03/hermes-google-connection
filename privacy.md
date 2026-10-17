---
title: Privacy — Nora Hermes Assistant
---

# Privacy and Google data handling

Last updated: 2026-10-17

This page describes the Google connection for a private, self-hosted installation
of Nora Hermes Assistant, administered by the person who invited its user.

## Access and use

The assistant accesses Google data only after the Google account holder grants
OAuth permission. Its connection requests Gmail mailbox access, access to calendar
events, and read-only access to the calendar list. These permissions support mail
search, summaries, drafting and sending mail, and reading or managing events in
response to user instructions or user-configured routines. This installation does
not request Google Drive, Contacts, Sheets or Docs access.

The administrator and anyone with access to the assistant's authorised account or
server may be able to access its stored data. This private installation is not a
service that isolates separate customers from the administrator.

## Storage and model processing

Google passwords are entered at Google and are not required by this API
connection. OAuth credentials and refresh tokens are stored on the private
assistant server with restricted file permissions. Access tokens can be renewed
using the granted refresh token until access expires or is revoked.

Relevant message or event content may be sent to the configured AI model provider
(currently OpenAI) to carry out the user's request. Provider processing and
retention depend on the configured service and account settings. The installation
itself uses models for inference and does not train general-purpose AI models.

Conversation history, tool results, summaries and user-directed memories may be
retained in the assistant's local data store. They can include information from
Google when needed for the requested assistant features. Retained information
remains until removed through the assistant or by its administrator; there is no
fixed automatic deletion period promised by this installation.

## Sharing and restrictions

The installation does not sell Google user data or use it for advertising. Data
is used for its user-facing personal assistant functions and is shared with the
configured processing providers only as needed for those functions. It is not
intended as a publicly accessible mailbox or calendar service.

Google API data use and transfer are subject to the
[Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy),
including its Limited Use requirements. The account holder should review the
assistant's model-provider settings with the administrator before connecting.

## Revoking access and deletion

The account holder can revoke the connection through
[Google Account third-party connections](https://myaccount.google.com/connections).
Revoking access stops new authorised API access; it does not automatically remove
information previously saved in assistant conversations or memories. Ask the
installation administrator to remove the Google credentials and any retained
Google-derived history or memories that should be deleted. Changes already made
to Gmail messages or calendar events remain in Google unless separately changed.

For privacy or deletion requests, contact the person who invited you to the
private installation directly. Do not send account data or credentials to public
GitHub issues. This documentation site is hosted by GitHub Pages and has no login
form, advertising scripts or application mailbox data.

[Back to the application description](index.html)
