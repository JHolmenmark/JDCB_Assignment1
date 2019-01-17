# JDCB_Assignment1

SQL code:

CREATE DATABASE sqlandjava;

CREATE TABLE `sqlandjava`.`people` (
  `person_id` INT NOT NULL,
  `firstname` VARCHAR(45) NOT NULL,
  `lastname` VARCHAR(45) NOT NULL,
  PRIMARY KEY (`person_id`));

INSERT INTO `sqlandjava`.`people` (`person_id`, `firstname`, `lastname`) VALUES ('1', 'Anna', 'Bolt');
INSERT INTO `sqlandjava`.`people` (`person_id`, `firstname`, `lastname`) VALUES ('2', 'Carl', 'Dolk');
INSERT INTO `sqlandjava`.`people` (`person_id`, `firstname`, `lastname`) VALUES ('3', 'Erik', 'Fram');
INSERT INTO `sqlandjava`.`people` (`person_id`, `firstname`, `lastname`) VALUES ('4', 'Gina', 'Hult');

CREATE USER user@localhost IDENTIFIED BY 'password';
GRANT SELECT ON sqlandjava.people TO super@localhost;
