<body>
<img src = "https://github-vistors-counter.onrender.com/github?username=https://github.com/HeiderJeffer/MSc-in-AI-ETH-ZURICH-and-USI-Ubiquitous-Computing" alt = "Visitors-Counter"/>
</body>

#### <span class="smallcaps">ETH Zurich and UNIVERSITÀ DELLA SVIZZERA ITALIANA</span>

#### FACULTY OF COMPUTER SCIENCE - Master in Artificial Intelligence

#### Topic: Ubiquitous Computing \[2014\]

#### Speaker: Heider Jeffer and Prof. Marc Langheinrich

#### Instructor: Mehdi Jazayeri

#### Assistant: Sasa Nesic



# Summary

Ubiquitous computing (ubicomp) is a post-desktop model of human-computer
interaction in which information processing has been thoroughly
integrated into everyday objects and activities. In the course of
ordinary activities, someone ”using” ubiquitous computing engages many
computational devices and systems simultaneously, and may not
necessarily even be aware that they are doing so. This model is usually
considered an advancement from the desktop paradigm.

This paradigm is also described as pervasive computing, ambient
intelligence. When primarily concerning the objects involved, it is also
physical computing, the Internet of Things, haptic computing, and things
that think. Rather than propose a single definition for ubiquitous
computing and for these related terms, a taxonomy of properties for
ubiquitous computing has been proposed, from which different kinds or
flavors of ubiquitous systems and applications can be described.

At their core, all models of ubiquitous computing (also called pervasive
computing) share a vision of small, inexpensive, robust networked
processing de- vices, distributed at all scales throughout everyday life
and generally turned to distinctly common-place ends. For example, a
domestic ubiquitous computing environment might interconnect lighting
and environmental controls with personal biometric monitors woven into
clothing so that illumination and heating conditions in a room might be
modulated, continuously and imperceptibly. Another common scenario
posits refrigerators ”aware” of their suitably-tagged contents, able to
both plan a variety of menus from the food actually on hand and warn
users of stale or spoiled food.

Ubiquitous computing presents challenges across computer science: in
systems design and engineering, systems modeling, and user interface
design. Contemporary human-computer interaction models, whether command-

line, menu-driven, or GUI-based, are inappropriate and inadequate to the
ubiquitous case. This suggests that the ”natural” interaction paradigm
appropriate to fully robust ubiquitous computing has yet to emerge -
although there is also recognition in the field that in many ways we are
already living in a ubicomp world. Contemporary devices that lend some
support to this latter idea include mobile phones, digital audio
players, radio-frequency identification tags, GPS, and interactive
whiteboards.

# Ubiquitous learning

For some, ubiquitous learning (or u-learning) is equivalent to some form
of simple mobile learning, e.g. that learning environments can be
accessed in various contexts and situations. A ubiquitous learning
environment is any setting in which students can become immersed in the
learning process. So, a ubiquitous learning environment /ULE/ is a
situation or set of pervasive /or omnipresent/ education /or learning/.
Education is happening all around the student but the student may not
even be conscious of the learning process. Source data is present in the
embedded objects and students do not have to DO anything to learn. They
just have to be there.

# Examples using Python:
These examples provide a basic implementation reflecting the concepts of ubiquitous computing and ubiquitous learning as described in the research paper. The implementations can be extended further based on specific functionalities and interactions envisioned in ubiquitous computing environments. Each section can be expanded with additional features and complexities depending on the depth required for my research and application development. To implement the research paper on Ubiquitous Computing in Python, I can break down the implementation into sections based on the topics mentioned: Ubiquitous Computing and Ubiquitous Learning (U-Learning). Here's a structured approach:

### 1. Ubiquitous Computing

#### Example Scenario:
Let's simulate a basic ubiquitous computing environment where a user interacts with various interconnected devices.

```python
class Environment:
    def __init__(self, room_name):
        self.room_name = room_name
        self.light = False
        self.temperature = 25  # in Celsius

    def adjust_lighting(self, intensity):
        if intensity > 0:
            self.light = True
        else:
            self.light = False

    def adjust_temperature(self, delta):
        self.temperature += delta

    def __str__(self):
        return f"Room: {self.room_name}\nLight: {'On' if self.light else 'Off'}\nTemperature: {self.temperature} °C"

# Usage example:
living_room = Environment("Living Room")
living_room.adjust_lighting(1)
living_room.adjust_temperature(-2)
print(living_room)
```

#### Explanation:
This code represents a basic model of a ubiquitous computing environment (a living room in this case). It demonstrates how a user could interact with devices that adjust lighting and temperature automatically based on user preferences or environmental conditions.

### 2. Ubiquitous Learning (U-Learning)

#### Example Scenario:
Implementing a simple model of ubiquitous learning where students learn passively from their environment.

```python
class Student:
    def __init__(self, name):
        self.name = name
        self.knowledge = 0

    def learn(self, environment):
        if environment.light:
            self.knowledge += 1
        if environment.temperature < 20:
            self.knowledge += 1

# Usage example:
alice = Student("Alice")
alice.learn(living_room)
print(f"{alice.name} gained knowledge: {alice.knowledge}")
```

#### Explanation:
This code simulates a student (Alice) who gains knowledge based on environmental factors such as lighting and temperature. In a ubiquitous learning scenario, students can learn without actively participating in traditional learning activities.
