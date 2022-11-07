
---

# Business Goal

> The platform must establish a way to incentivize and create connections between police and members of the community through selfies for change; the proof of concept for the mobile platform. However, selfies are not required for the platform. Instead we simply want community members to approach and say Hello to an officer, while performing a virtual handshake. 

## Architecturally significant requirements

| # | Architecturally significant requirements | Business Goal |
|----|----|----|
| 1     | Cross-platform                                | 1 |
| 2     | User profile                                  | 1 |
| 3     | Geolocation                                   | 1 |
| 4     | Opt-in push nofications                       | 1 |
| 5     | Points                                        | 1, 2 |
| 6     | Rewards catalog                               | 2 |
| 7     | Analytics                                     | 1, 2 |

Based on the listed architecturally significant requirements, we can create the following functional and non-functional requirements.

## Functional Requirements
### FR001 Cross-platform
The platform must be accessible from both web and mobile devices.

### FR002 User Profile
All platform users can create a profile.

Police officers (SH-2) must have ability to use their work email address.

Civilians (SH-1) must have ability to create a profile with social media integration. Civilians can only link 1 email address to a particual phone device. Multiple device registration is prohibited.

Both non-profit organizations (SH-3) and for-profit organizations (SH-4) can create a profile.

### FR003 Geolocation
Platform users' location is used for finding connections between civilans (SH-1) and police officers (SH-2) therefore their location is tracked all the time.

Geofencing must be used as a connection can only happen if civilian (SH-1) and police officer (SH-2) are within a 10 ft (3 m) distance from each other.

To protect police officers (SH-2), their location sharing must automatically shut off after 15 minutes.

Police officers (SH-2) should not find other members of the platform. 

When civilans (SH-1) have opt-ed in push notifications (FR004), they should be notificed for pariticatping for-profit organization (SH-4) near them.

### FR004 Opt-in push notifications
Both civilians and police officers get notified when an opportunity for an interaction with between them is nearby.

Platform users must have ability to opt-in or opt-out from push notifications.

Civilians (SH-1) can opt-in for push notifications when participating for-profit organizations (SH-4) is near them.

### FR005 Points
Both civilans (SH-1) and police officers (SH-2) collect points for each interactions that can be redeemed or donated.

Only 1 connection can happen between a private citizen and per police officer within 24 hour period.

Non-profit organizations (SH-3) must have ability to receive points donation.

### FR006 Rewards catalog
As system users gain points for interactions, both non-profit (SH-3) and for-profit organizations (SH-4) should have ability to create a storefront when they list rewards which can be redeemed by civilians (SH-1) and police officers (SH-2). 


## FR007 Analytics
Connections between civilans and police officers must be tracked.

Every police officer must have a count that displays how many connections they have made.


## Non-Functional Requirements

### NFR001 Ease of use
Users should fulfill their taks in the system with ease.

### NFR002 Accessiblity
The platform should be usable by everyone in the community.

### NFR003 Scalability
The platform should scale as the amount of users increase.