# 配置中心

CREATE TABLE `config_properties` (
  `id` bigint NOT NULL AUTO_INCREMENT,
  `key` varchar(50) CHARACTER SET utf8 COLLATE utf8_bin NOT NULL,
  `value` varchar(500) CHARACTER SET utf8 COLLATE utf8_bin DEFAULT NULL,
  `application` varchar(50) CHARACTER SET utf8 COLLATE utf8_bin NOT NULL,
  `profile` varchar(50) CHARACTER SET utf8 COLLATE utf8_bin NOT NULL,
  `label` varchar(50) CHARACTER SET utf8 COLLATE utf8_bin DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

insert into `config_properties` (`id`, `key`, `value`, `application`, `profile`, `label`) values('1','server.port','8083','config-client','dev','master');
insert into `config_properties` (`id`, `key`, `value`, `application`, `profile`, `label`) values('2','foo','bar-jdbc','config-client','dev','master');