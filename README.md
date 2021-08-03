#-- phpMyAdmin SQL Dump
-- version 5.1.1
-- https://www.phpmyadmin.net/
--
-- Host: 127.0.0.1
-- Tempo de geração: 03-Ago-2021 às 05:37
-- Versão do servidor: 10.4.20-MariaDB
-- versão do PHP: 8.0.8

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Banco de dados: `agricode`
--

-- --------------------------------------------------------

--
-- Estrutura da tabela `cliente`
--

CREATE TABLE `cliente` (
  `id` int(40) NOT NULL,
  `nome` varchar(40) NOT NULL,
  `senha` varchar(40) NOT NULL,
  `email` varchar(40) NOT NULL,
  `dtnasc` date NOT NULL,
  `usuario` varchar(40) NOT NULL,
  `ss_temp` varchar(40) NOT NULL,
  `ss_umidade` varchar(40) NOT NULL,
  `ss_chuva` varchar(40) NOT NULL,
  `ss_nivelagua` varchar(40) NOT NULL,
  `ss_chamas` varchar(40) NOT NULL,
  `bomba_agua` varchar(40) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Extraindo dados da tabela `cliente`
--

INSERT INTO `cliente` (`id`, `nome`, `senha`, `email`, `dtnasc`, `usuario`, `ss_temp`, `ss_umidade`, `ss_chuva`, `ss_nivelagua`, `ss_chamas`, `bomba_agua`) VALUES
(112457845, 'Roberto Felipe', '123456', 'feliperoberto@gmail.com', '2003-10-03', 'RobertoPlantation', '26º', '69%', 'Não', 'Médio', 'Não', 'Desligada');

--
-- Índices para tabelas despejadas
--

--
-- Índices para tabela `cliente`
--
ALTER TABLE `cliente`
  ADD PRIMARY KEY (`id`);

--
-- AUTO_INCREMENT de tabelas despejadas
--

--
-- AUTO_INCREMENT de tabela `cliente`
--
ALTER TABLE `cliente`
  MODIFY `id` int(40) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=112457846;
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
