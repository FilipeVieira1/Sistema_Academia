CREATE TABLE Aluno (
    id_aluno INT PRIMARY KEY,
    nome VARCHAR(100),
    cpf CHAR(11) UNIQUE,
    data_nascimento DATE,
    telefone VARCHAR(15),
    email VARCHAR(120),
    status_plano VARCHAR(20)
);

CREATE TABLE Professor (
    id_professor INT PRIMARY KEY,
    nome VARCHAR(100),
    cpf CHAR(11) UNIQUE,
    cref VARCHAR(15),
    especialidade VARCHAR(80),
    telefone VARCHAR(15),
    email VARCHAR(120)
);

CREATE TABLE Plano (
    id_plano INT PRIMARY KEY,
    nome_plano VARCHAR(50),
    valor DECIMAL(10,2),
    dias INT
);

CREATE TABLE Contrato (
    id_contrato INT PRIMARY KEY,
    id_aluno INT,
    id_plano INT,
    data_inicio DATE,
    data_fim DATE,
    status VARCHAR(20),
    FOREIGN KEY (id_aluno) REFERENCES Aluno(id_aluno),
    FOREIGN KEY (id_plano) REFERENCES Plano(id_plano)
);

CREATE TABLE Pagamento (
    id_pagamento INT PRIMARY KEY,
    id_contrato INT,
    data_pagamento DATE,
    valor_pago DECIMAL(10,2),
    forma_pagamento VARCHAR(30),
    status_pagamento VARCHAR(20),
    FOREIGN KEY (id_contrato) REFERENCES Contrato(id_contrato)
);

CREATE TABLE Treino (
    id_treino INT PRIMARY KEY,
    nome_treino VARCHAR(80),
    data_criacao DATE,
    id_professor INT,
    id_aluno INT,
    FOREIGN KEY (id_professor) REFERENCES Professor(id_professor),
    FOREIGN KEY (id_aluno) REFERENCES Aluno(id_aluno)
);

CREATE TABLE Exercicio (
    id_exercicio INT PRIMARY KEY,
    nome_exercicio VARCHAR(80),
    tipo VARCHAR(50),
    musculo_principal VARCHAR(50)
);

CREATE TABLE Treino_Exercicio (
    id_treino INT,
    id_exercicio INT,
    series INT,
    repeticoes INT,
    carga INT,
    descanso INT,
    PRIMARY KEY (id_treino, id_exercicio),
    FOREIGN KEY (id_treino) REFERENCES Treino(id_treino),
    FOREIGN KEY (id_exercicio) REFERENCES Exercicio(id_exercicio)
);

CREATE TABLE Checkin (
    id_checkin INT PRIMARY KEY,
    id_aluno INT,
    data_hora_checkin DATETIME,
    FOREIGN KEY (id_aluno) REFERENCES Aluno(id_aluno)
);
