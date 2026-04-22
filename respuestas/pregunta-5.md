MATCH (p:Persona)-[:TRABAJA_EN]->(e:Empresa) MATCH (p)-[:VIVE_EN]->(c:Ciudad) RETURN p.nombre, e.nombre, c.nombre
