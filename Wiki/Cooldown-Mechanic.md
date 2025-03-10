@@ -5,7 +5,7 @@ An advanced spell casting and cooldown handler using Auras and VariableSkills. A reliable casting handler for player casting.

## Attributes
| Attribute | Aliases   | Description                                                          | Default |
|-----------|-----------|----------------------------------------------------------------------|---------|
| id   | cast, spell | The delay in seconds before a spell is cast.                        | 1 |
| name   | spellname | The damage threshold required to interrupt Channelling.                      | 2 |
| spellcooldown   | spellcd | Metaskill to execute upon begining Channelling.                     | channel-start_fx |
| displaycooldown   | displaycd, showcd |  Metaskill to execute on tick while Channelling.                        | channel-tick_fx |

## Examples
  cooldown-cast-1:
    Skills:
    - skill{s=spell-cast;
      name="Test Shot";id=test-shot-fire;
      origin=@SelfEyeLocation{fo=-0.5;yo=-0.2};
      spellcooldown=2;damage=2.5} @ENO{r=24}

  cooldown-cast-2:
    Skills:
    - skill{s=spell-cast;
      name="Chain Shot";id=test-chainmissile-cast;
      spellcooldown=10} @self

  cooldown-cast-3:
    Skills:
    - skill{s=spell-charge-cast;branch=true;
      name="Spiral Shot";
      id=test-spiralshot-fire;
      origin=@SelfEyeLocation{fo=-0.5;yo=-0.2};
      spellcooldown=0.5;
      chargecooldown=4;charges=3} @forward{f=12;uel=true}

