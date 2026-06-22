# Router Drop

Router dropping describes the method of using multiple players carrying different construction modules
being flown out via ESF or Valkyire to quickly build small construction outposts within the vicinity of 
facilities to be attacked.

It's main advantage lies in its speed, as the previous step of pulling ANTs to harvest cortium usually
falls out.

!!! info "Prerequisites"
    Having unlocked <b>Logistics certifications I</b> are required to conduct basic variations of the router drop.

## Basic variant (Duo)

The easiest way to cover most key concepts regarding router dropping is to go over it's most basic variant including 
two players.

### Aquiring modules

Construction modules can be aquired from <b>cortium silo terminals</b> or from <b>deployed ANTs</b>. The absolute minimum 
amount of modules required for aquiring a router are the <b>routing spire</b> as well as a nearby <b>cortium silo</b> to 
power it.

<!--=== "Image: Terminals"-->

![Screenshot](assets/constructionterminals.webp)
!!! warning "Silo storage & reserved mode"
     Cortium silos feature an indicator for their amount of stored cortium. Should the amount of cortium drop below a certain threshold <i>(less than 4 squares on the indicator)</i>, the silo will enter reseved mode and bar access to any player that <b>isn't in a squad with the silos constructor</b>!

<!--=== "Image: Construction Menu"-->

![Screenshot](assets/constructionmenu.webp)
!!! info "Construction menu navigation"
    The <b>cortium silo</b> can be found within the <b>CORE</b> tab. The routing spire is located under <b>SPIRES</b>. Click the star icon located within the yellow circle to favourite the modules, causing them to be listed in <b>FAVOURITES</b>.

<!--=== "Image: Holding module"-->

![Screenshot](assets/holdingmodule.webp)
!!! failure "Global NDZ-Bug"
    Should you get a promt saying "you are in a no-deploy zone" despite being outside the red circles drawn within the minimap, you unfortunately have contracted the <b>global no-deploy zone</b> bug which requires you to restart the game before being able to place any construction modules.


<div style="
    float:right;
    margin:0 1.5rem 1rem 0.5rem;
    border:1px solid var(--md-default-fg-color--lightest);
    border-radius:1px;
    padding:2rem 1rem;
    text-align:center;
    box-shadow:0 1px 2px rgba(0,0,0,.1);
">
  <img src="../assets/commandcenter.webp" alt="commandcenter.webp">
</div>

Sufficiently filled cortium silos are usually found at larger construction bases further away from the frontlines. 
A good tip would be to search for <b>command centers</b> within the map screen's spawn list.

Obviously spawns provided by <b>rebirthing centers</b> or <b>elysium spawn tubes</b> can also have well filled cortium silos nearby. Note that listed spawn entries 
feature small icons depicting which terminals are nearby for use:

<div style="
  border:1px solid var(--md-default-fg-color--lightest);
  border-radius:8px;
  padding:1rem;
  text-align:center;
  box-shadow:0 2px 4px rgba(0,0,0,.1);
">
  <img src="../assets/commandcenter2.webp" alt="commandcenter.webp">
</div>

!!! note "Aircraft terminal availability"
    It generally is recommended to source construction modules from bases which feature local aircraft terminals. That way aircraft can be pulled quickly at a discounted nanite cost in order to fly out the modules to the desired location.


### Conducting the Router drop

The average procedure which plays out in most router drops is laid out in the flow chart below. For clarity's sake, follow along the <b><span style="color:#ffaa00">tan colored</span></b> path as it lays out a router drop procedure with no complications coming up.

Cells containing an information symbol <b>ⓘ</b> have annotations below proving further context. 

```mermaid
graph TB
  A(Locate Silo)
  B{<b><span style="font-size:32px">ⓘ</span></b><br>Verify absence of global NDZ}
  C[Grab Silo and Spire]
  D[Restart the Game]
  E[Fly to a 500m vicinity of facility to be attacked]
  F{Too close to other deployables?}
  G[Place Modules]
  H(Spire player grabs and places router)

  I[<b><span style="font-size:32px">ⓘ</span></b><br>Mark Silo with STO]
  J[Find another drop location]
  L[<b><span style="font-size:32px">ⓘ</span></b><br>Destroy enemy spire and replace it with your own <b>parasitic spire</b>]


  A --> B
  B -->|no bug present| C
  C -->|for squad leads| I 
  B -->|NDZ-bug present| D
  D --> B
  C --> E
  E --> F
  F -->|Yes, allied base obstructing <b>OR</b> guarded enemy base| J
  J --> G
  F -->|Yes, unguarded enemy base obstructing| L
  L --> G
  F -->|no nearby deployables| G
  G -->|Modules finished constructing?| H

  classDef main fill:#ffe1a6,stroke:#000000;
  class A,B,C,E,F,G,H main;

  linkStyle 1 stroke:#000000,stroke-width:4px;
  linkStyle 0 struoke:#000000,stroke-width:4px;
  linkStyle 5 stroke:#000000,stroke-width:4px;
  linkStyle 6 stroke:#000000,stroke-width:4px;
  linkStyle 11 stroke:#000000,stroke-width:4px;
  linkStyle 12 stroke:#000000,stroke-width:4px;
```

??? info "Verifying global NDZ abscence"
    bruh

??? info "Squad Tactical Overlays (STO's)"
    nerd shit

??? info "Parasitic routing spires"
    how rude

### Consecutive Drops

Functional construction modules such as silos and spires have adjacency limitations as well as being limited to <b>one placed module per character</b>.

<table>
  <thead>
    <tr>
      <th></th>
      <th align="center">Iteration 1</th>
      <th align="center">Iteration 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
       <td style="text-align:center; vertical-align:middle;">Player 1</td>
      <td align="center">
        <img src="../assets/Cortium_Silo.webp" alt="Cortium Silo"><br>
        Cortium Silo
      </td>
      <td align="center">
        <img src="../assets/Routing_Spire.webp" alt="Routing Spire"><br>
        Routing Spire
      </td>
    </tr>
    <tr>
       <td style="text-align:center; vertical-align:middle;">Player 2</td>
      <td align="center">
        <img src="../assets/Routing_Spire.webp" alt="Beispiel 1"><br>
        Routing Spire
      </td>
      <td align="center">
        <img src="../assets/Cortium_Silo.webp" alt="Beispiel 2"><br>
        Cortium Silo
      </td>
    </tr>
  </tbody>
</table> 

### Router Network

### Post-Plant

## Advanced Variants (3+ Players)

### Construction drop coordinator