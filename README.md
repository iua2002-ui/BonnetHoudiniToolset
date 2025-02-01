# README: Digital Toolset for Art-Directable Hair, Braid, and Curl Generation in Houdini

### **Project Overview**
This project presents a digital toolset created for art-directable hair braid and curl generation in Houdini. It is an independent, self-taught initiative aimed at providing a more inclusive approach to hair representation in digital content. The toolset is designed with a focus on creating hair for culturally diverse characters, especially those with Black and POC backgrounds, by incorporating a variety of braid and curl styles. The goal is to allow artists to generate realistic, adjustable hair patterns and styles while enhancing the representation of diverse hair textures in digital animation and modeling.

### **Inspiration**
- **Disney BDRF Tool**: This tool was adapted to accommodate POC character features, as seen in films like *Encanto* and *Soul*. This project expands on that idea by creating tools that start with diversity as a core feature.
- **Theodore Kim’s 2022 SIGGRAPH Talk**: Inspired by the notion of rethinking character representation, particularly with inclusive practices, this project aims to make diversity foundational in digital asset creation rather than an additive component.
- **Diversity in Feature Studios**: While major studios often add diversity-inclusive technology to existing pipelines, the goal of this project is to rethink the design of digital tools where diversity is the basis, increasing suitable representation for Black and POC characters.

### **Key Features**
- **Art-Directable Hair Creation**: The toolset allows for the generation of diverse braid and curl patterns, offering control over hair texture, color, and styling.
- **Braids and Box Braids**: The tool generates braids around guide curves procedurally, accommodating different curl patterns and diverse braiding styles.
- **Adjustable Parameters**: Users can control varying curl patterns, hair color, and styling to reflect cultural diversity.
  
### **Technical Details**
- **VEX Code Integration**: The hair and braid patterns are defined using VEX code within Houdini. The tool uses mathematical computations to generate the curl and braid patterns based on guide curves.
- **Guide Curve System**: Hair patterns are procedurally generated on guide curves, which define the shape and flow of the hair. The system allows for visualizing hair on any primitive within Houdini.
  
### **Core Components**
- **Wrangle Node**: A custom wrangle node defines the guide curve vector and assigns the value in the Y-axis property. The node retrieves points from resampled guide curves, computes the correct orientation for the X and Y axes, and assigns tangent vectors accordingly.
- **Skin Hairs**: Density attributes are painted and scattered to mark hair growth on the scalp. A script creates primitives based on the closest braid guide curves, then connects iterated points to form hairs that grow into the braid.
- **Copy to Points**: A scatter node assigns points to geometry, translating to the points defined on braid primitives. The result is individual hairs output on the braid structure.

### **Examples**
- **Afro Hairstyle Simulation**: The tool can simulate an afro hairstyle using Houdini's hair system, allowing for the creation of realistic curls.
- **Poly Wire Braid**: An example of a poly wire braid built on a curve, demonstrating how the tool can generate braid patterns procedurally.

### **Goals and Objectives**
1. **Procedural Braiding**: Generate box braids and other diverse braiding styles procedurally around guide curves.
2. **Varying Curl Patterns**: Incorporate varying curl patterns, from loose waves to tight curls, into the procedural generation.
3. **Hair Customization**: Allow adjustable parameters for hair color, texture, and style, ensuring a diverse representation of hair textures and cultural styles.
4. **Inclusive Digital Assets**: Provide digital tools that enhance the representation of Black and POC characters in CGI and digital art, ensuring accurate and respectful depictions of hair.

### **Usage**
This toolset can be used by digital artists and studios looking to incorporate culturally diverse hair styles in their digital characters. It can be utilized in projects that require procedurally generated hair, with adjustable styles for a more inclusive representation of Black and POC characters.

### **Contributions**
This project is an ongoing exploration of digital asset creation for more inclusive character representation. Contributions and feedback from artists, programmers, and storytellers who are passionate about diverse representation are encouraged.

### **Contact**
For any inquiries or contributions, please contact [Your Name] at [Your Email].

---

This README summarizes the project’s objective, key features, technical aspects, and the overall goal of enhancing diverse representation in digital assets, particularly for hair styling in 3D animation and modeling.
