
# YouTube Skeleton Clone 
## Introduction

This document describes the design of a simplified YouTube clone. The goal of this project is not to build a 1 to 1 clone of YouTube, but rather to build a rough skeleton where the core functionality of YouTube is implemented.

We are focused on keeping the design as simple as possible, while still addressing some scalability tradeoffs. We are focused on learning, not building a production ready system.

## Background 

YouTube is a video sharing platform that allows users to upload, view, rate, share, and comment on videos.

The scope of YouTube is very large, such that even "trivial" features like rating and commenting on videos are actually quite complex at this scale (1B+ daily active users). For this reason, we will be focusing mostly on uploading videos, and a bit on viewing videos.
## High Level Design

<img width="1053" alt="image" src="https://github.com/bhavy2202/YouTube-Skeleton-Clone/assets/114098067/d3a82031-df55-4920-bbb0-ae4474ee0d00">

## requirement 

>Users can sign in/out using their Google account

>Users can upload videos while signed in

>Videos should be transcoded to multiple formats (e.g. 360p, 720p)

>Users can view a list of uploaded videos (signed in or not)

>Users can view individual videos (signed in or not)

## References
Firebase Auth: https://firebase.google.com/docs/auth

Cloud Storage Signed URLs: https://cloud.google.com/storage/docs/access-control/signed-urls

Pub/Sub Push subscriptions: https://cloud.google.com/pubsub/docs/push

Using Pub/Sub with Cloud Storage: https://cloud.google.com/storage/docs/pubsub-notifications

Using Pub/Sub with Cloud Run: https://cloud.google.com/run/docs/tutorials/pubsub

