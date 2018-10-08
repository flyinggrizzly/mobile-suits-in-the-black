---
title: The Resistance
shipDescription: |
  A ship struggling to gather resources and unite friends and former enemies to
  oppose a corrupt government. Examples from different Gundam series include the
  _Argama_ from _Mobile Suit Zeta Gundam_, the Delaz fleet from _Mobile Suit
  Gundam 0083: Stardust Memories_, and the _Garencieres_ from _Mobile Suit
  Gundam Unicorn_.
type: ship
resources:
  tier_1:
    - name: ship
      description: |
        The ship you rely on to wage your righteous war. It is your home, your
        base of operations, and the thing that allows you to fight against the
        corruption.
    - name: Mobile Suit complement
      description: |
        The mobile suits you begin with. You can choose either:

        - A few old mass-production mobile suits you have acquired as
        out-of-date surplus, or that you have maintained since the last war

        - Some new top of the line performance suits, that will give you an
        edge, but be much harder to maintain

        If you need another complement of mobile suits, securing this resource a
        second time gains you five mass-production MS (more performance suits
        will require a **materiel supplier**).
    - name: Pilot squad
      description: |
        A squad of 5 pilots who can back you up on sorties. Name each
        of them, give them heritages and backgrounds, and describe where you met
        them.
      benefit: You have more qualified pilots aiding you.
      strings: |
        You must pay the pilots 1 FK each downtime, and when you do not mark
        a tick on a 6-clock. If the clock fills, you must pay them 8 FK before
        they will fly for you again.
    - name: Mechanic corps
      description: |
        You recruit a dedicated maintenance team to help maintain your crew's
        mobile suits.
      benefit: |
        Your crew gains 1 free downtime action, which must be spent on repairing
        your mobile suits.
      strings: |
        You must pay the mechanics 1 FK each downtime, and when you do not mark
        a tick on a 6-clock. If the clock fills, you must pay them 8 FK before
        they will work on your mobile suits again.
  tier_2:
    - name: Sister organization
      description: |
        Another group somewhere fighting towards the same goals. Their strength
        matches yours, and they will grow as you grow as you do. They might be
        an earth-bound group if you are in space, or vice versa. The
        relationship in _Mobile Suit Zeta Gundam_ between the AEUG and Karaba is
        very much what this is like.
      benefit: |
        Gain a bonus die for engagement rolls when your mission relies on their
        support.
      strings: |
        Add **Ally under attack** to your fallout table.
    - name: Financial backer
      description: |
        A wealthy patron sympathetic to your cause and willing to underwrite
        your efforts. They might be backing you because fighting corruption is
        the right thing to do, or just because they have selfish interests that
        align with your goals. The relationship between Luio & Co and the AEUG
        in _Mobile Suit Zeta Gundam_ is a good point of reference. When you win
        this resource, describe your backer (are they a wealthy individual, a
        company, or something else?), and their reason for backing you. This
        should be a specific reason, whether selfish or altruistic.
      benefit: 8 FK per downtime
      strings: |
        When the actions your crew takes frustrate or deviate from your
        patron's goals, mark a tick on a 4-clock. When it is full they will
        withdraw their support unless you undertake a mission to appease them.
  tier_3:
    - name: Materiel supplier
      description: |
        An arms manufacturer that is capable of supplying your crew with new and
        better arms and equipment.
      benefit: |
        Gain one new performance mobile suit per crew member/player when you
        secure this resource. If any of your crew members are an Ace or a
        Newtype, they may instead choose a unique or custom unit. Additionally,
        you have easier access to materiel: all repairs cost 1 FK less, and
        repairs on performance or custom MS only require 1 downtime action since
        you no longer have to manufacture the parts yourself.
      strings: |
        The military industrial complex is huge, amorphous, and foul. Add
        **Leaks** to the list of entanglements. Someone in your supplier is
        playing both sides. If you roll this entanglement, you are immediately
        attacked by your enemy (before downtime actions begin). Treat this
        attack as another mission (including normal engagement procedure).
    - name: Political standing
      description: |
        You have grown strong enough to be recognized as, or insist on being
        recognized as a legitimate political actor, not jut an insurgency. In
        _Mobile Suit Zeta Gundam_, this is the moment when Bajeena speaks before
        the UN.
      benefit: |
        When you retaliate for an attack by your enemy, your engagement roll
        begins at 1d6, and you do not need to stake resources on it.
      strings: |
        If any of your allies take an action that is contrary to what your
        political stance is understood to be, you must either declare them
        anathema and lose their resource, or lose this resource. In the public
        eye you do not have the benefit of compromise.
fallout:
  frict_5:
    one:
      available: true
      name: Engine trouble
      description: |
        Something goes very wrong with your engines or some other critical ship
        system. You can repair this as usual, but the lack of power is something
        you're going to have to deal with. It may cause you problems on your
        next engagement roll if you've having to travel far (-1 die).
    two:
      available: true
      name: Run-in on neutral territory
      description: |
        While you are out on R&R after your mission, you run into an enemy or
        rival. Make a fortune roll:

          - 1-3: they have seen you and are making a move
          - 4-5: you have the advantage if you want to attack or trail them, but
              you have to _act now_ without time to prepare
          - 6: you have the advantage
          - Crit: They've already slipped up and given you something. What is
              it?
    three:
      available: true
      name: Reprisal
      description: |
        The enemy is on you. Pay 2 FK to have an ally intercept them or bog them
        down with bureaucracy, or deal with them yourself.
    four:
      available: true
      name: Defector
      description: |
        Someone from your enemy has appeared claiming to be a defector.
    five:
      available: true
      name: Aid needed
      description: |
        One of your allies needs your aid. The GM will tell you what kind
        (military, financial, technical, logistical, etc). You can dispatch one
        of your cohort resources like Pilot squad or Mechanics corps to aid if
        appropriate. If you do not help them now, you cannot use them as a
        staked resource until you deliver this aid, or make up for not helping
        them when they needed it.
    six:
      available: true
      name: Mobile suit trouble
      description: |
        The repairs on your mobile suits are going to be more difficult than you
        thought. You must either pay 4 FK to get them repaired rapidly, or do
        without them on your next mission. If you didn't use your mobile suits
        at all in the last mission, you avoid fallout for now.
  frict_8:
    one:
      available: true
      name: Captured by a rival
      description: |
        One of the PCs is captured by the enemy. Did it happen when everyone
        thought they were safe after the last mission and returning to base? Was
        the PC careless on shore-leave? A player should volunteer their
        character for capture. Instead of normal downtime activities, play out a
        scene with the character and their rival.

        Until the crew decides to mount a rescue mission (or the character finds
        another way out), the player should play as a different character during
        missions. You can (and should!) still have scenes about this character
        while they're captive during downtimes. This can be a great way to
        elaborate on a relationship with your rival, or even convince them to
        change sides.
    two:
      available: true
      name: Neutral state under threat
      description: |
        The enemy is trying to get a foothold in some place that has worked to
        remain neutral through this conflict. They have explicitly asked you not
        to come to their home, but if you leave the enemy to continue, the
        neutral state will become embroiled against their will. And they will be
        against you...
    three:
      available: false
      name: Ally under attack
      description: |
        When you roll this fallout, if you do not come immediately to your
        ally's aid, you will lose this resource.
    four:
      available: true
      name: Defection
      description: |
        A member of your crew or a close ally defects to your enemy. What pushed
        them to betray you?
    five:
      available: true
      name: Rival trouble
      description: |
        Someone's rival corners them. Where and how? Are they attacking, or is
        there something they want?
    six:
      available: false
      name: entanglement six
  frict_10:
    one:
      avaiable: true
      name: entanglement 1
    two:
      available: true
      name: Roll on the 0-5 friction table
    three:
      available: true
      name: fallout three
    four:
      available: false
      name: fallout four
    five:
      available: false
      name: Leaks
      description: |
        Someone in your materiel supplier is playing both sides. If you roll
        this fallout, you are immediately attacked by your enemy (before
        downtime actions begin). Treat this attack as another mission (including
        normal engagement procedure).
    six:
      available: false
      name: fallout six

---

{{% notice note %}}
The clocks you may need to keep track of for the Resistance are:

- a 4-clock representing your financial backer's dissatisfaction with your
    actions
- 6-clocks for missing payments to Pilots or Mechanics
- any playbook specific clocks, like those started by the [Rookie's]({{< ref
    "/playbooks/rookie.md#move_letters-home-starting-move" >}}) **Letters home** ability
{{% /notice %}}
