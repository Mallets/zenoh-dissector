# Zenoh Dissector
[Zenoh](http://zenoh.io/) protocol dissector for Wireshark

## Under devopment

- [ ] Zenoh Messages
  - [x] Declare
      - [x] Resource Declaration
      - [x] Publisher Declaration
      - [x] Subscriber Declaration
      - [x] Queryable Declaration
      - [ ] Forget Resource
      - [x] Forget Publisher
      - [ ] Forget Subscriber
      - [ ] Forget Queryable
  - [x] Data
  - [ ] Query
  - [ ] Pull
  - [ ] Unit
  - [ ] Link State List
- [ ] Session Messages
  - [ ] Scout
  - [ ] Hello
  - [x] Init
  - [x] Open
  - [x] Close
  - [ ] Sync
  - [ ] Ack Nack
  - [x] Keep Alive
  - [x] Ping Pong
  - [x] Frame
- [ ] Decorators Messages
  - [ ] Routing Context
  - [ ] Reply Context
  - [ ] Attachment
- [x] Decode Frame message (including several messages)
  - [x] Support Frame fragmentation
- [x] Decode multiple Zenoh messages in a single TCP message
  - [x] Handle Zenoh messages split across TCP messages
- [ ] Message filtering for framed messages
- [ ] Implement unit tests
- [ ] Extensive Testing

## Usage

To use this, copy zenoh.lua to ~/.local/lib/wireshark/plugins.
Then when you run Wireshark it will understand TCP/UDP communications
on port 7447 as Zenoh messages, and will know how to interpret them. 

## License
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
