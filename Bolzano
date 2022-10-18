'''

Teorema de Bolzano

'''

from matplotlib import pyplot as plt

def f(x):
    return '''Insertar aquí la función'''
   
a = '''Insertar aquí el valor inferior'''
b = '''Insertar aquí el valor superior'''
margen = 0.01
x = range(a, b+1)

if f(a) * f(b) < 0:
    while abs(f((a+b)/2)) >= margen:
        c = (a+b)/2
        if f(c) == 0:
            print('f(x) = 0 en x = '+ str(round(c,2)))
            break
        if f(a) * f(c) < 0:
            b = c
        else:
            a = c
    mensaje = ('f(x) = 0 en x = '+ str(round(c,2)))
    print(mensaje)
    ''' La función plotfunc() contiene el código para graficar la función '''
    def plotfunc():
        plt.plot(x, [f(i) for i in x])
        plt.scatter(c, f(c))
        plt.title(mensaje)
        plt.axhline(0, color="black")
        plt.axvline(0, color="black")
        # plt.xlim([-10, 10])
        # plt.ylim([-10,10])
        plt.show()
    plotfunc()
else:
    print('No se puede aplicar el teorema de Bolzano en el intervalo ' + str(a) + ', ' + str(b))    
