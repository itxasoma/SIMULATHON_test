This simulation implements the Vicsek model to study the behaviour of a flock of birds. In a nutshell: Simple local rules lead to global collective motion. It's a basic but powerful model for understanding how groups of things can self-organize and move together, like birds flocking or fish schooling. A scarecrow is implemented to see the interaction of the flock with an external stimulus that breaks the collective motion.

How to:
- Move the cursor over the canvas to control the scarecrow.
- Click to scare nearby birds and activate the sound.
  
Parameters:
- Average velocity of the center of mass: Imagine you find the exact middle point of the whole group of moving particles. Its speed tells you how fast the entire group is moving together in a specific direction.
VCM = (1/N) * Σ (vi)
  N = total number of particles
  vi = velocity vector of the i-th particle
  Σ = sum over all particles
- Global order (polarization): Think of it like a group dance. If everyone is moving in almost the same direction, the dance is very ordered. Polarization measures how "in sync" all the particles are in their movement direction, from perfectly aligned to completely random.
φ = | (1/N) * Σ (v̂i) |
  N = total number of particles
  v̂i = *unit* velocity vector of the i-th particle
  Σ = sum over all particles
  | ... | = magnitude of the vector
  
Sound characteristics:
- Each bird has a note associated with its direction in Lydian mode (mapped to C3, C4, C5).
- Clicking the scarecrow plays a low C (triangle synth).
- Birds affected by the sound wave play their notes according to their direction.
  
...

Credits: Itxaso Muñoz-Aldalur (GitHub: itxasoma).

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

