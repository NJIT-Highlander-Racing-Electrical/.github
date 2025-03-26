# Lessons Learned during 2024-2025 season

## Enclosures

### Modeling Dimensions

Since all of the enclosures are relatively the same, it would have been much easier to have one master template with variables for length, width, and height dimensions that could easily be changed for each subsystem to accomodate different sized PCBs

### Gaskets

The gasket material we used this year was a bit annoying to work with. Because it has a fabric-y feel, it was hard to laser cut cleanly. It also did not adhere to the acrylic covers with superglue very well because the superglue absorbed into the material.

### Cover Screws

Two things to do with this. One, a screw on top and bottom instead of just the sides would have been beneficial so the acrylic doesnt arch in the middle. Additionally, some of the screw threads got messed up when making them into thumb screws, so maybe find a better way to attach the plastic knobs for that 

### Laser Cutting Enclosures

The power setting seemed to be just shy of where it needed to be. Some enclosures cut perfectly fine, but there were other parts where the very bottom was not fully cut through and some post-processing had to be done

### Spray Painting Enclosurse

Most turned out very nice. One thing to make sure of is that any tape covering areas not to be spray painted is fully pressed down with a large overlap so no paint bleeds into those regions

### Laser Cutting Engraving Board

Engraving board was very annoying to get tuned in this year. See [Dashboard Manufacturing Doc](https://docs.google.com/document/d/1SboHkU5eu9X-XPbC42ve_8zeORpnQzHskEh5Oi-o60I/edit?usp=drive_link)


## Electronics Hardware

### Adafruit CAN Pal Transceivers

Definitely had some issues with these over the last two years. Mysterious issues that are hard to pinpoint. Ethan found some with poor soldering jobs on the SMD components, so perhaps their quality control is not too good. Additioanlly, the through hole mounting is extremely hard to replace. Maybe our custom surface mount ones next year may be easier to replace if necessary, or we can find ways to make the larger components modular (like multi-pin ICs)


## Brake Light

Our old circular brake light was outdated, so I was looking to upgrade to something more modern. Polaris offers several brake lights, but it does not look like they sell the connectors for them. I (wrongly) assumed it was just a standard 3-pin way connector, but it turned out to be a proprietary connector. So, I ordered the proprietary connectors on Amazon, and then soon discovered that Polaris uses more than one proprietary connector! It appears that SAE does not permit any brake lights with the connectors I ordered, so I modified an existing 3-pin way connector to fit the brake light's notches. Functionally the same, but worth noting this extra step in the assembly process. I have also made 2-3 extra modified connectors as spares or for future years. I still think it is worth sticking with our current 2411450 brake light model. 
