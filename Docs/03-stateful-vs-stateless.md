# Stateful vs Stateless Firewall 

## Stateless Firewall

- Examines packets individually
- No memory of previous packets
- Faster but less secure

Used in basic packet filtering.


## Stateful Firewall

- Tracks connection state
- Understands session context
- Allows return traffic automatically

More secure and commonly used.


## Key Difference

Stateless: "Is this packet allowed?"
Stateful: "Does this packet belong to a valid session?"

Modern firewalls are almost always stateful.
