-- phpMyAdmin SQL Dump
-- version 5.2.1
-- https://www.phpmyadmin.net/
--
-- Servidor: 127.0.0.1
-- Tiempo de generación: 25-06-2026 a las 18:16:44
-- Versión del servidor: 10.4.32-MariaDB
-- Versión de PHP: 8.2.12

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Base de datos: `zapateria_adoc`
--

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `clientes`
--

CREATE TABLE `clientes` (
  `id_Cliente` int(11) NOT NULL,
  `Nombre` varchar(50) NOT NULL,
  `Apellido` varchar(50) NOT NULL,
  `Télefono` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Volcado de datos para la tabla `clientes`
--

INSERT INTO `clientes` (`id_Cliente`, `Nombre`, `Apellido`, `Télefono`) VALUES
(1, 'Carlos', 'González', 70112233),
(2, 'María', 'Rodríguez', 71223344),
(3, 'Juan', 'López', 72334455),
(4, 'Ana', 'Martínez', 73445566),
(5, 'Luis', 'Pérez', 74556677),
(6, 'Carmen', 'Gómez', 75667788),
(7, 'José', 'Sánchez', 76778899),
(8, 'Elena', 'Fernández', 77889900),
(9, 'Francisco', 'Ramírez', 78990011),
(10, 'Isabel', 'Torres', 79001122),
(11, 'Jorge', 'Díaz', 60112233),
(12, 'Martha', 'Vásquez', 61223344),
(13, 'Pedro', 'Castro', 62334455),
(14, 'Sofía', 'Morales', 63445566),
(15, 'Miguel', 'Herrera', 64556677),
(16, 'Lucía', 'Jiménez', 65667788),
(17, 'Roberto', 'Aguilar', 66778899),
(18, 'Laura', 'Salazar', 67889900),
(19, 'Alejandro', 'Delgado', 68990011),
(20, 'Claudia', 'Mendoza', 69001122),
(21, 'Ricardo', 'Ramos', 70224466),
(22, 'Patricia', 'Cruz', 71335577),
(23, 'Fernando', 'Ortiz', 72446688),
(24, 'Gabriela', 'Flores', 73557799),
(25, 'David', 'Guzmán', 74668800);

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `productos`
--

CREATE TABLE `productos` (
  `id_Producto` int(11) NOT NULL,
  `id_proveedor` int(11) NOT NULL,
  `Nombre` varchar(50) NOT NULL,
  `Descripción` text NOT NULL,
  `Precio` decimal(10,0) NOT NULL,
  `Stock` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Volcado de datos para la tabla `productos`
--

INSERT INTO `productos` (`id_Producto`, `id_proveedor`, `Nombre`, `Descripción`, `Precio`, `Stock`) VALUES
(1, 1, 'Zapato Escolar Clásico', 'Zapato negro de cuero para colegio', 25, 50),
(2, 1, 'Mocasín Formal Negro', 'Calzado formal de vestir para caballero', 45, 30),
(3, 2, 'Tenis Deportivo Running', 'Zapatillas ligeras para correr, color azul', 60, 40),
(4, 2, 'Tenis Casual Blanco', 'Tenis urbanos de lona para el día a día', 35, 60),
(5, 3, 'Bota Industrial de Seguridad', 'Bota con punta de acero de alta resistencia', 55, 20),
(6, 3, 'Bota Vaquera de Cuero', 'Bota de piel estilo vaquero color café', 85, 15),
(7, 4, 'Sandalia Playera', 'Sandalia cómoda y fresca de hule para verano', 12, 100),
(8, 4, 'Pantufla de Descanso', 'Pantufla abrigadora de felpa para el hogar', 15, 45),
(9, 5, 'Tacón de Aguja Elegante', 'Zapatos de tacón alto para fiesta color rojo', 50, 25),
(10, 5, 'Zapatilla Flat Casual', 'Calzado bajo y cómodo para dama', 22, 70),
(11, 1, 'Tenis de Basket Alta', 'Zapatos deportivos con soporte de tobillo', 75, 18),
(12, 1, 'Zapato Casual Oxford', 'Zapato semi-formal de cuero sintético', 40, 35),
(13, 2, 'Bota de Lluvia Impermeable', 'Bota de hule alta para temporada invernal', 28, 30),
(14, 2, 'Zapato de Plataforma Dama', 'Calzado moderno con plataforma de corcho', 42, 22),
(15, 3, 'Zapatilla de Ballet Confort', 'Calzado ultra flexible para danza o uso diario', 18, 40),
(16, 3, 'Alpargata de Lona', 'Calzado fresco con suela estilo yute', 20, 55),
(17, 4, 'Zapato de Golf Profesional', 'Calzado técnico con tacos para tracción', 95, 10),
(18, 4, 'Botín de Gamuza Café', 'Botines de otoño con cierre lateral', 48, 25),
(19, 5, 'Zapato Clínico Blanco', 'Calzado cómodo ideal para enfermería o médicos', 32, 50),
(20, 5, 'Chancla Deportiva', 'Chancla ligera para baño o piscina', 10, 120),
(21, 1, 'Zapato Escolar Dama', 'Zapato escolar tipo guillermina', 24, 40),
(22, 2, 'Tenis Skate Urbano', 'Tenis de suela plana para patinar', 45, 30),
(23, 3, 'Bota de Montaña Trekking', 'Bota impermeable para senderismo', 70, 15),
(24, 5, 'Tacón Bloque Confort', 'Tacón medio cuadrado para oficina', 38, 28),
(25, 1, 'Tenis Infantil Luces', 'Tenis divertidos con luces led en la suela', 29, 35);

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `proveedores`
--

CREATE TABLE `proveedores` (
  `id_proveedor` int(11) NOT NULL,
  `Nombre` varchar(50) NOT NULL,
  `Apellido` varchar(50) NOT NULL,
  `Télefono` int(11) NOT NULL,
  `Correo` varchar(50) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Volcado de datos para la tabla `proveedores`
--

INSERT INTO `proveedores` (`id_proveedor`, `Nombre`, `Apellido`, `Télefono`, `Correo`) VALUES
(1, 'Calzado', 'Mendoza', 71234567, 'ventas@calzadomendoza.com'),
(2, 'Distribuidora', 'Gómez', 72345678, 'contacto@distgomez.com'),
(3, 'Cueros', 'Alvarado', 73456789, 'alvaradocueros@gmail.com'),
(4, 'Suelas', 'Hernández', 74567890, 'suelashernandez@outlook.com'),
(5, 'Manufacturas', 'López', 75678901, 'mlopez_fabrica@hotmail.com');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `usuarios`
--

CREATE TABLE `usuarios` (
  `id_usuarios` int(11) NOT NULL,
  `Usuario` enum('Adminstrador','Empleado') NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Volcado de datos para la tabla `usuarios`
--

INSERT INTO `usuarios` (`id_usuarios`, `Usuario`) VALUES
(1, 'Adminstrador'),
(2, 'Empleado'),
(3, 'Empleado'),
(4, 'Empleado');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `ventas`
--

CREATE TABLE `ventas` (
  `id_Ventas` int(11) NOT NULL,
  `id_cliente` int(11) NOT NULL,
  `id_usuario` int(11) NOT NULL,
  `id_producto` int(11) NOT NULL,
  `cantidad` int(11) NOT NULL,
  `Total` decimal(10,0) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Volcado de datos para la tabla `ventas`
--

INSERT INTO `ventas` (`id_Ventas`, `id_cliente`, `id_usuario`, `id_producto`, `cantidad`, `Total`) VALUES
(1, 3, 2, 1, 2, 50),
(2, 5, 3, 3, 1, 60),
(3, 1, 2, 7, 3, 36),
(4, 8, 4, 2, 1, 45),
(5, 12, 3, 5, 2, 110),
(6, 2, 2, 10, 1, 22),
(7, 15, 4, 9, 1, 50),
(8, 20, 2, 4, 2, 70),
(9, 7, 3, 20, 4, 40),
(10, 11, 4, 6, 1, 85),
(11, 4, 2, 12, 1, 40),
(12, 9, 3, 16, 2, 40),
(13, 18, 4, 11, 1, 75),
(14, 25, 2, 19, 1, 32),
(15, 14, 3, 8, 2, 30),
(16, 6, 4, 14, 1, 42),
(17, 22, 2, 25, 2, 58),
(18, 13, 3, 23, 1, 70),
(19, 19, 4, 18, 1, 48),
(20, 21, 2, 15, 3, 54),
(21, 10, 3, 22, 1, 45),
(22, 17, 4, 24, 1, 38),
(23, 23, 2, 13, 2, 56),
(24, 16, 3, 17, 1, 95),
(25, 24, 4, 21, 2, 48);

--
-- Índices para tablas volcadas
--

--
-- Indices de la tabla `clientes`
--
ALTER TABLE `clientes`
  ADD PRIMARY KEY (`id_Cliente`);

--
-- Indices de la tabla `productos`
--
ALTER TABLE `productos`
  ADD PRIMARY KEY (`id_Producto`),
  ADD KEY `id_provedor` (`id_proveedor`);

--
-- Indices de la tabla `proveedores`
--
ALTER TABLE `proveedores`
  ADD PRIMARY KEY (`id_proveedor`);

--
-- Indices de la tabla `usuarios`
--
ALTER TABLE `usuarios`
  ADD PRIMARY KEY (`id_usuarios`);

--
-- Indices de la tabla `ventas`
--
ALTER TABLE `ventas`
  ADD PRIMARY KEY (`id_Ventas`),
  ADD KEY `id_cliente` (`id_cliente`),
  ADD KEY `id_usuario` (`id_usuario`),
  ADD KEY `id_producto` (`id_producto`);

--
-- AUTO_INCREMENT de las tablas volcadas
--

--
-- AUTO_INCREMENT de la tabla `clientes`
--
ALTER TABLE `clientes`
  MODIFY `id_Cliente` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=26;

--
-- AUTO_INCREMENT de la tabla `productos`
--
ALTER TABLE `productos`
  MODIFY `id_Producto` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=26;

--
-- AUTO_INCREMENT de la tabla `proveedores`
--
ALTER TABLE `proveedores`
  MODIFY `id_proveedor` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=6;

--
-- AUTO_INCREMENT de la tabla `usuarios`
--
ALTER TABLE `usuarios`
  MODIFY `id_usuarios` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=5;

--
-- AUTO_INCREMENT de la tabla `ventas`
--
ALTER TABLE `ventas`
  MODIFY `id_Ventas` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=26;

--
-- Restricciones para tablas volcadas
--

--
-- Filtros para la tabla `productos`
--
ALTER TABLE `productos`
  ADD CONSTRAINT `productos_ibfk_1` FOREIGN KEY (`id_proveedor`) REFERENCES `proveedores` (`id_proveedor`);

--
-- Filtros para la tabla `ventas`
--
ALTER TABLE `ventas`
  ADD CONSTRAINT `ventas_ibfk_1` FOREIGN KEY (`id_cliente`) REFERENCES `clientes` (`id_Cliente`),
  ADD CONSTRAINT `ventas_ibfk_2` FOREIGN KEY (`id_producto`) REFERENCES `productos` (`id_Producto`),
  ADD CONSTRAINT `ventas_ibfk_3` FOREIGN KEY (`id_usuario`) REFERENCES `usuarios` (`id_usuarios`);
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
