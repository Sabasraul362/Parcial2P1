public class Alumno {

 /**
 *
 * @author Sabas
 */
public String getNombre() {
return nombre;
}
 
public String getClases() {
return clases;
}
 
public String getGrado() {
return grado;
}
 
public String getGrupo() {
return grupo;
}
 
public void setNombre(String nombre) {
this.nombre = nombre;
}
 
public void setClases(String clases) {
this.clases = clases;
}
 
public void setGrado(String grado) {
this.grado = grado;
}
 
public void setGrupo(String grupo) {
this.grupo = grupo;
}
private String nombre;
private String clases;
private String grado;
private String grupo;
 
protected void ir_a_clase(){
 
}
 
protected void estudiar(){
 
}
}

public class Regular extends Alumno{
 
public Regular(){
 
}
 
protected void pagar_inscripcion(){
 
}
 
protected void matricularse(){
 
}
}


2
3
4
5
6
7
8
9
10
public class Becario extends Alumno{
 
public Becario(){
 
}
 
protected void pagar_inscripcion(){
 
}
}


2
3
4
5
6
7
8
9
10
11
12
13
public class Intercambio extends Alumno{
 
public Intercambio(String nombre,String clases,String grado,String grupo){
super.setNombre(nombre);
super.setClases(clases);
super.setGrado(grado);
super.setGrupo(grupo);
}
 
protected void matricularse(){
 
}
}

public class Main {
public static void main(String args[]){
Regular pepe = new Regular();
pepe.setNombre("Pepe");
pepe.setClases("Biologia,matematicas");
pepe.setGrado("2");
pepe.setGrupo("G");
pepe.ir_a_clase();
 
Intercambio luis = new Intercambio("Luis","Fisica,Ecologia","3","B");
luis.ir_a_clase();
luis.estudiar();
luis.matricularse();
}
}
