para as tabelas no mysql workbench


create database banco_exemplo;

CREATE TABLE Alunos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    nota1 DECIMAL(4,2),
    nota2 DECIMAL(4,2),
    nota3 DECIMAL(4,2),
    nota4 DECIMAL(4,2),
    media DECIMAL(4,2),
    situacao VARCHAR(100)
);

CREATE TABLE ParImpar(
id INT AUTO_INCREMENT PRIMARY KEY,
numero INT,
classificacao VARCHAR(10)
);

create table MaiorIdade(
id int auto_increment primary key,
idade int,
acesso VARCHAR(20)
);


create table TrianguloValido(
id int auto_increment primary key,
lado_a int,
lado_b int,
lado_c int,
tipo varchar(50)
);

create table Reajuste(
id int auto_increment primary key,
salario_original decimal(10,2),
percentual int,
valor_aumento decimal(10,2),
salario_final decimal(10,2)
);

CREATE TABLE IMC (
    id int auto_increment primary key,
    peso decimal(5,2),
    altura decimal(4,2),
    imc decimal(5,2),
    categoria varchar(50)
);

CREATE TABLE AnoBissexto (
    id int auto_increment primary key,
    ano int,
    resultado varchar(30)
);

CREATE TABLE Emprestimo (
    id INT AUTO_INCREMENT PRIMARY KEY,
    valor_casa DECIMAL(12,2),
    salario DECIMAL(10,2),
    anos INT,
    prestacao_mensal DECIMAL(10,2),
    resultado VARCHAR(30)
);


CREATE TABLE NatacaoCategoria (
    id INT AUTO_INCREMENT PRIMARY KEY,
    ano_nascimento INT,
    idade INT,
    categoria VARCHAR(20)
);

CREATE TABLE LojaTintas (
    id INT AUTO_INCREMENT PRIMARY KEY,
    area DECIMAL(10,2),
    litros_necessarios DECIMAL(10,2),
    latas INT,
    preco_total DECIMAL(10,2)
);
