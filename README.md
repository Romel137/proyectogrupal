# 🩺 Sistema de Turnos Médicos

Este proyecto es una aplicación web desarrollada con **Django** que permite la **gestión y reserva de turnos médicos** entre pacientes y doctores, organizados por especialidades. La solución está orientada a consultorios, clínicas pequeñas o instituciones que requieran un sistema simple pero efectivo para gestionar la disponibilidad médica.

---

## 🎯 Objetivo del Proyecto

El objetivo principal es ofrecer una plataforma digital que:

- Automatice la reserva de turnos entre pacientes y profesionales de la salud.
- Evite la sobrecarga de personal administrativo gestionando reservas de manera manual.
- Controle la disponibilidad médica en función de día y hora.
- Permita escalabilidad futura con funcionalidades como recordatorios por correo electrónico.

---

## 🧩 Estructura del Proyecto

El sistema se compone de las siguientes entidades principales:

- **Paciente**: Usuario registrado con rol de paciente. Puede reservar turnos.
- **Doctor**: Usuario con especialidad médica. Puede recibir turnos y ser visualizado por los pacientes.
- **Especialidad**: Rama médica (p. ej., Pediatría, Cardiología) que clasifica a los doctores.
- **Turno**: Registro de una cita entre un paciente y un doctor en una fecha y hora específica.

---

## 🛠️ Tecnologías Utilizadas

- **Python 3** y **Django**
- **SQLite** como base de datos por defecto
- **HTML** y **Django Templates** para la parte visual
- **Autenticación de usuarios** (registro, login y logout)
- **Sistema de roles**: Paciente / Doctor
- **Validación de turnos duplicados**
- **Correo electrónico** (estructura base para recordatorios, aún por implementar)

---

##  Funcionalidades
✅ Para los Pacientes:
Registro como paciente.

Visualización de la lista de doctores por especialidad.

Reserva de turnos disponibles por fecha y hora.

Visualización de turnos propios.

Validación para evitar superposición de turnos.

Recibirá notificaciones por email (estructura implementada, envío aún pendiente de configurar completamente).

✅ Para los Doctores:
Registro como doctor con especialidad médica.

Gestión automática de su disponibilidad (no se permite agendar turnos repetidos).

Visualización de turnos asignados en su perfil (en construcción).
