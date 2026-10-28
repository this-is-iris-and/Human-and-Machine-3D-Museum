# Human and Machine: Art Style Plan

Virtual museum · 3D Modelling for Real-Time Applications (HSLU) · Paule-Iris Djeni

**The museum title is open on purpose.** "Human and Machine" can mean a human separate from a machine, or a human and a machine as one thing. The three halls lead the visitor from the first reading to the second.

| Stage | Hall | What it means |
| --- | --- | --- |
| Human **and** Machine, apart | Looking Behind | The machine is a separate tool. The human picks it up, uses it and puts it down. |
| Human **with** Machine, together | Looking Around | The machine is a companion. It is light and smart, and we take it everywhere, but it is still a separate object. |
| Human **as** Machine, one | Looking Forward | There is no clear line any more. The machine is merged with the human body. |

## Art style: Tool, Companion, Self

Stylized to semi-real, with three distinct halls and no nature or greenery theme. Across the halls, machines move from tools we use when we need them, to companions we take everywhere, to something merged with the human body.

| Hall | Time | Idea | Look |
| --- | --- | --- | --- |
| Looking Behind | 1950s onwards | Tool | Big machines that we use when we need them. Warm, retro, colourful plastics and wood. |
| Looking Around | Today | Companion | White and grey, minimal, Apple-style. Small devices with tiny colour accents. |
| Looking Forward | Unknown future | Self | Light, airy and almost empty. The machine is part of the human body. Calm and warm, like the film *Her* (2013, directed by Spike Jonze), not cyberpunk. |

**Why this name.** In the 1950s machines were tools that stayed in one place: a phone you could not carry, a desk calculator, a typewriter, a radio, each doing one job. Today light, smart devices are companions we take everywhere. In the future, chips in the body remove the border between us and the machine, and the tool becomes part of the self.

**The Cloud.** The biggest piece of Looking Forward stands in the centre of the hall. We do not all fully trust big tech, but we still let them access our data and devices, and maybe soon our whole life and body, if we have chips integrated into it.

**Motif: the forgotten.** History is told through the middle and ruling class. The poor and lower middle class are rarely talked about and their traces disappear. Each hall has one dusty, worn piece that stands for these people, shown with dignity.

## Colour palette (60-30-10)

| Hall | 60% | 30% | 10% |
| --- | --- | --- | --- |
| Looking Behind | cream `#F2E3CF` | warm wood `#8B5E3C` | orange `#E8742C`, red `#D8402E`, teal `#5FA8A0` |
| Looking Around | soft white `#F2F2EF` | greys `#C9CCCF`, `#8E9399` | signal orange `#FF5A1F`, tiny primaries `#E63B2E`, `#F2C230`, `#2F6BFF` |
| Looking Forward | warm light `#F6EEE6` | skin tones `#E8B79A`, `#D9A58C` | coral `#D9573F` (sparingly) |
| The Cloud | pale sky blue glow `#BFE3F2` | white haze | none |
| The forgotten pieces | dust grey-brown `#8C7F72` | rust `#9A5B3C` | none |

No pure white or black on big surfaces. The pale blue of the Cloud is used nowhere else.

## Shaders for XR

1. **Baked material:** lighting saved in the textures, used for most objects.
2. **Soft glow:** for the Cloud, lights and screens.
3. **Colour blend:** a smooth change from a human colour to a machine colour, where the boundary blurs.

All three are cheap enough for a standalone Meta Quest 3.

## Texture and mesh limits

Target: Meta Quest 3, standalone. These are first estimates.

| Item | Limit |
| --- | --- |
| Triangles (the small shapes a 3D model is made of), whole scene | under 1.5M (course limit), aiming well below |
| Textures | up to 2048 px for main pieces, smaller for the rest |

## Mood board

The school version has a full collage with five groups (A to E) and two hero images. This repository only links **free-licence** images. Protected images (Pinterest collections, film stills, art installations) are not part of it.

| Group | Image | Credit and licence |
| --- | --- | --- |
| A. Looking Behind | [Sony Walkman TPS-L2 (1979)](https://solarspell-dls.sfis.asu.edu/mea/wikipedia/images/2319/231971.jpg.htm) | Døgen, Wikimedia Commons, CC BY-SA 2.0 |
| A. Looking Behind | [Braun World Receiver T 1000 (1963)](https://brooklynmuseum.org/opencollection/objects/170035) | Dieter Rams design, Brooklyn Museum, CC-BY |
| D. The forgotten | [Abandoned room with peeling wallpaper](https://unsplash.com/photos/abandoned-room-with-peeling-wallpaper-K5sjajgbTFw) | Nolan Issac, Unsplash License |
| D. The forgotten | [Abandoned rustic kitchen](https://unsplash.com/photos/abandoned-rustic-kitchen-with-old-stove-and-chairs-J6T78kdQXIQ) | Peter Herrmann, Unsplash License |
| D. The forgotten | [Old building, broken window, peeling paint](https://unsplash.com/photos/an-old-building-with-a-broken-window-and-peeling-paint-0NQMdLYnLI4) | Ibrahim guetar, Unsplash License |

Group E (real-time look) is my own Twinmotion gallery scene, built from a Twinmotion template with people and objects added.

Still missing free sources: white and minimal devices, a warm airy interior, a chip implant, soft cloud-like light.

## AI use

The concept and the writing are mine. I used an AI assistant to sort my notes, suggest colour palettes and check that the plan fits the assignment.
