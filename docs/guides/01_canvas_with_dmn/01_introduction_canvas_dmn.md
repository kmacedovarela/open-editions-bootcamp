# Canvas & Decision Model and Notation (DMN) 

## The Value of Open Standards for Decision Automation

### Why DMN, and What is it

Decision Model and Notation (DMN) is an open standard that provides a powerful framework for decision automation. It offers a visual notation for decision modeling, a standardized approach to defining decision logic, and ensures interoperability between different tools and platforms. Designed to be easily understood by all stakeholders, from business users to developers, DMN enables the creation of executable models that can be run on various platforms, ensuring consistent decision-making processes.

DMN is particularly valuable because it:
- Enhances communication between business and technical teams through visual notation
- Ensures consistency and clarity in decision logic across different systems
- Facilitates sharing and reuse of models across various tools and platforms
- Supports a wide range of decision logic, from simple rules to complex decision trees

### FEEL: A Standard Friendly Enough Expression Language

FEEL (Friendly Enough Expression Language) is a key component of DMN that provides an intuitive way to express decision logic. Here are some examples of FEEL to give you an idea of its simplicity:

**Simple Conditional Logic**: Checking if an applicant's age is above 18:

```
if applicant.age > 18 then "Eligible" else "Not Eligible"
```

**String Manipulation**: Concatenating the first name and last name of an applicant:

```
applicant.firstName + " " + applicant.lastName
```

**List Operations**: Calculating the average score from a list of scores:

```
sum(scores) / count(scores)
```

**Date Operations**: Calculating the number of days between two dates:

```
days between startDate and endDate
```

## IBM & OMG: Working towards the evolution of DMN

The collaboration between IBM and the Object Management Group (OMG) has been instrumental in the development and evolution of DMN. This partnership ensures continuous improvement of the standard, alignment with industry needs, and broader adoption across various sectors.

!!! question "Did you know"

      The team behind Drools, an open-source decision management system, has been actively involved with OMG since the early days of DMN. They have consistently implemented the standard, even in its early versions. For more detailed information on Drools' implementation of DMN, you can [explore Drools' documentation](https://docs.drools.org/latest/drools-docs/drools/DMN/index.html).


---

Next, let's explore the development experience with Canvas, starting with connecting Canvas to OpenShift.

## Development Experience with Canvas

!!!note

      If you haven't installed Canvas yet, please follow the installation guide here: [Installing Canvas on OpenShift](../00_intro/04_env_setup#installing-canvas-on-openshift)

### Connecting Canvas to GitHub

To connect BAMOE Canvas to GitHub, follow these steps:

1. **Create a GitHub Personal Access Token:**
    - Go to [GitHub Settings](https://github.com/settings/tokens)
    - Click on "Generate new token"
    - Select the required scopes for accessing your repositories
    - Generate the token and copy it

2. **Configure Canvas with GitHub Token:**
    - Access BAMOE Canvas web interface
    - Go to Settings
    - Enter your GitHub personal access token in the provided field
    - Save the configuration

With these steps, BAMOE Canvas will be connected to your GitHub account, allowing you to import projects and synchronize your work.

---

:material-check-circle-outline: _Great job! You now have a solid understanding of DMN and its value in decision automation. Let's dive into the development experience with Canvas._

---