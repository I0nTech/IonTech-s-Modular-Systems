Dependencies:
- MM Premium (latest build)
- Crucible (For items)
- ModelEngine (For Model Modules, optional for all others.)
- PlaceholderAPI
  - Expansions:
    - Math
    - String

In MythicMobs/Config/config-skills.yml, set TargetArmorStands & TargetMarkers = true
Then reload.

Install and reload PAPI, then:

In Plugins/placeholderAPI/config.yml
Copy and paste this in, replace/add to bottom of string if present:

  string:
    replacements:
      cleanup:
        '_': ""
      small-text:
        '0': ₀
        '1': ₁
        '2': ₂
        '3': ₃
        '4': ₄
        '5': ₅
        '6': ₆
        '7': ₇
        '8': ₈
        '9': ₉
        a: ᴀ
        b: ʙ
        c: ᴄ
        d: ᴅ
        e: ᴇ
        f: ғ
        g: ɢ
        h: ʜ
        i: ɪ
        j: ᴊ
        k: ᴋ
        l: ʟ
        m: ᴍ
        n: ɴ
        o: ᴏ
        p: ᴘ
        q: ǫ
        r: ʀ
        s: s
        t: ᴛ
        u: ᴜ
        v: ᴠ
        w: ᴡ
        x: x
        y: ʏ
        z: ᴢ
      small-numbers:
        '0': ₀
        '1': ₁
        '2': ₂
        '3': ₃
        '4': ₄
        '5': ₅
        '6': ₆
        '7': ₇
        '8': ₈
        '9': ₉
    separator: _

