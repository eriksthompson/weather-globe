🌍 Weather Globe

Weather Globe is a real-time, interactive 3D visualization of global weather conditions built with React, 
Three.js (via React Three Fiber), and a Node.js backend. The application renders a fully rotatable and zoomable
Earth with dynamic day/night lighting, seasonal sun positioning, and night city lights using custom GLSL shaders. 
Live precipitation data is mapped to geographic coordinates and visualized directly on the globe as rain, snow, cloud
cover, and active storm systems.

The backend aggregates forecast data from the Open-Meteo API using a configurable latitude/longitude grid. To operate
within API limits, the service batches requests in chunks, throttles calls to prevent rate limiting, and caches results
in memory. Forecast data is refreshed at scheduled intervals and served instantly to the frontend via a lightweight REST
endpoint. This architecture ensures efficient API usage, stable performance, and scalable weather rendering without triggering 
excessive external requests.

The frontend focuses on geospatial accuracy and visual clarity. Storm intensity is classified server-side and rendered client-side
as layered atmospheric systems above the Earth’s surface. The project demonstrates full-stack architecture design, API 
rate-limit management, shader-based lighting systems, coordinate mapping from spherical geometry, and real-time 3D 
visualization techniques. Weather Globe serves as a strong portfolio example of combining backend data engineering with 
advanced interactive graphics.
