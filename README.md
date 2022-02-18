
                               - Desafio de Programação Academia Capgemini
                               
  
                                                   Questão 1
                                                   
                                                   
  Scanner entrada = new Scanner(System.in);
List<String> degraus = new ArrayList<>();

 
System.out.print("9");
int qtdDegraus = entrada.nextInt();

 
for (int i = 0; i < qtdDegraus; i++) {
degraus.add(" ".repeat(qtdDegraus - i) + "*".repeat(i + 1));
}

 
for (String d : degraus ) {
System.out.println(d);
}}


                                                   Questão 2

<label>Senha:</label>
<input type="password" id="password" minlength="6" maxlength="10" onKeyUp="verificaForcaSenha();" />
<span id="password-status"></span>


<script
  src="https://code.jquery.com/jquery-3.5.1.min.js"
  integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0="
  crossorigin="anonymous">
</script>


<script>
function verificaForcaSenha() 
{
	var numeros = /([0-9])/;
	var alfabeto = /([a-z,A-Z])/;
	var chEspeciais = /([~,!,@,#,$,%,^,&,*,-,_,+,=,?,>,<])/;

	if($('#password').val().length<6) 
	{
		$('#password-status').html("<span style='color:red'>Fraco, insira no mínimo 6 caracteres</span>");
	} else {  	
		if($('#password').val().match(numeros) && $('#password').val().match(alfabeto) && $('#password').val().match(chEspeciais))
		{            
			$('#password-status').html("<span style='color:green'><b>Forte</b></span>");
		} else {
			$('#password-status').html("<span style='color:orange'>Médio, insira um caracter especial</span>");
		}
	}
}
</script>


                                            Questão 3
                                            
                                      
for i in range(len(s2)):
        pos = ord(s2[i])-ord('a')
        c2[pos] = c2[pos] + 1

    j = 0
    aindaOK = True
    while j<26 and aindaOK:
        if c1[j]==c2[j]:
            j = j + 1
        else:
            aindaOK = Falsedef solucao(s1,s2):
    c1 = [0]*26
    c2 = [0]*26

    for i in range(len(s1)):
        pos = ord(s1[i])-ord('a')
        c1[pos] = c1[pos] + 1


    return aindaOK

print(solucao('muro','rumo'))

----------------------------------------////////------------------------------------
Questões 1 Java
Questão 2 em JavaScript
Questão 3 Python
