# GNS - Gamelan Notation Standard

GNS is a standard for gamelan notation based on Kepatihan system. This is early version of the standard.

## Root object

Consists of the version and the licence.

    "version": "v0.0.1",
    "licence": "MIT",

## Sections

Consists of array of section.

    "sections": [
        {
            "type": "title",
            "contents": {
                "type": "Jineman",
                "name": "Mari Kangen",
                "laras": "Slendro",
                "pathet": "Sanga"
            }
        },

### Section

Consists of type, array of contents, or array of lines.
Array of contents for type title:

            "type": "title",
            "contents": {
                "type": "Jineman",
                "name": "Mari Kangen",
                "laras": "Slendro",
                "pathet": "Sanga"
            }

Array of lines:

            "type": "celuk",
            "lines": [
                {
                    "gatra": [
                        {
                            "content": []
                        },
                        {
                            "content": []
                        },
                        {
                            "content": []
                        },
                        {
                            "content": [
                                {
                                    "number": ".",
                                    "attributes": []
                                },
                                {
                                    "number": ".",
                                    "attributes": []
                                },
                                {
                                    "number": ".",
                                    "attributes": []
                                },
                                {
                                    "number": "2",
                                    "attributes": ["kempul"]
                                }
                            ]
                        }
                    ]
                }
            ]
        },

### Lines

Consists of array of gatra:

            "lines": [
                {
                    "gatra": [
                        {
                            "content": [
                                {
                                    "number": "5",
                                    "attributes": []
                                },
                                {
                                    "number": "6",
                                    "attributes": []
                                },
                                {
                                    "number": "2",
                                    "attributes": []
                                },
                                {
                                    "number": "1",
                                    "attributes": ["kempul"]
                                }]
                        }
                    ]
                },


#### Gatra

Consists of gatra object, which has number and attributes.

                       {
                            "content": [
                                {
                                    "number": "5",
                                    "attributes": []
                                },
                                {
                                    "number": "6",
                                    "attributes": []
                                },
                                {
                                    "number": "2",
                                    "attributes": []
                                },
                                {
                                    "number": "1",
                                    "attributes": ["kempul"]
                                }]
                        }

#### Gatra attributes

A string-based name of attributes.

gong_gede = O surrounded the number
gong_suwuk = ( ) surrounded the number
kempul = > ontop, clockwise
kenong = < ontop, clockwise
kethuk = + ontop
kempyang = - ontop 
top_dot = an octabe higher
bottom_dot = an octave lower

# Sources

http://www.gamelan.org/library/fonts/KepatihanPro%20Keycaps.pdf
https://www.jstor.org/stable/1513116
https://en.wikipedia.org/wiki/Gamelan_notation
https://en.wikipedia.org/wiki/American_Gamelan_Institute
https://gamelan.gs/release/i-classical-gendings/
https://issuu.com/soni.petrovski/docs/marc_benamou_-_rasa__affect_and_intuition_in_javan