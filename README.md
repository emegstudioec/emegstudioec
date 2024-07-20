from graphviz import Digraph  

dot = Digraph(comment='Ética en la Inteligencia Artificial')  

dot.node('A', 'Ética en la Inteligencia Artificial')  
dot.node('B', 'Definición')  
dot.node('C', 'Privacidad y Seguridad')  
dot.node('D', 'Responsabilidad y Rendición de Cuentas')  
dot.node('E', 'Transformación de Sectores')  
dot.node('F', 'Riesgos de Prejuicios y Desigualdades')  
dot.node('G', 'Normativas y Recomendaciones')  
dot.node('H', 'Recursos Adicionales')  
dot.node('I', 'Impacto Social y Económico')  

dot.edges(['AB', 'AC', 'AD', 'AE', 'AF', 'AG', 'AH', 'AI'])  
dot.edge('B', 'C')  
dot.edge('B', 'D')  
dot.edge('B', 'E')  
dot.edge('B', 'F')  
dot.edge('G', 'H')  
dot.edge('G', 'I')  

dot.render('mapa_mental', format='png', cleanup=True) 
