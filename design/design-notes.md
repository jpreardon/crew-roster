# Design Notes

I've been curious about [AWS](https://aws.amazon.com/) for a while. I've done some tutorials and I even ran a Jamulus server a few times, but I haven't built anything as of yet. So, this is a first attempt. It's a simple app, hopefully not too aggressive for a dilettante like me.

There are some extremely basic [wireframes](crew-roster-wireframes.pdf) that show the screen flow. Some key aspects are missing from them, like administration/user management. That might come later, if this project actually goes anywhere. For now, I'm just going to concentrate on creating a RESTful API that supports what's in those wireframes.

## Data Points

All of these points should have created and updated datetimes.

- Skipper
  - Name
  - Email
  - Mobile Phone
  - Contact Preference (SMS/Email)
  - Vessels
- Crew
  - Name
  - Email
  - Mobile Phone
  - Contact Preference (SMS/Email)
- Vessel
  - Skipper
  - Name
  - Type (Sail/Power)
  - Length
  - Make
  - Model
- Crew Request
  - Vessel
  - Departure Datetime
  - Arrival Datetime
  - Number of Crew Needed
  - Crew
  - Special
  - Notes
- Crew Available
  - Departure Datetime
  - Arrival Datetime
  - Crew Name
  - Notes