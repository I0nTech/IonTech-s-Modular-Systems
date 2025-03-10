@@ -5,7 +5,7 @@ Cast in style. Extends Cooldown-Mechanics and inherits all parameters.

## Attributes
| Attribute | Aliases   | Description                                                          | Default |
|-----------|-----------|----------------------------------------------------------------------|---------|
| warmup   | duration, d | The delay in seconds before a spell is cast.                        | 1 |
| interrupt   | | The damage threshold required to interrupt Channelling.                      | 2 |
| onStart   | os | Metaskill to execute upon begining Channelling.                     | channel-start_fx |
| onTick   | ot |  Metaskill to execute on tick while Channelling.                        | channel-tick_fx |
| onInterrupt   | oi |  Metaskill to execute when Channelling is interrupted.                | channel-interrupt_fx |
| onCast   | oc |  Metaskill to execute before Casting.                    | channel-cast_fx |

## Examples
  channel-test_cast: #For testing only.
    Skills:
    - skill{s=channel;
      name=Mana Blast;id=manablast-exec;
      warmup=3;spellcooldown=8}

