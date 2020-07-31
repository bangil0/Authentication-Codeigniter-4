# Authentication Codeigniter 4 With Mitos\Auth

## Use Mitos\Auth

Flexible, Powerful, Secure auth package for CodeIgniter 4.
[official site](https://github.com/lonnieezell/myth-auth).

## Installation
Installation is best done via Composer. Assuming Composer is installed globally, you may use the following command:

`> composer require myth/auth`

## Configuration Validation.php
Edit app/Config/Validation.php and add the following value to the ruleSets array: 

`\Myth\Auth\Authentication\Passwords\ValidationRules::class`

## Configuration Filters.php
First, edit application/Config/Filters.php and add the following entries to the aliases property:

`'login'      => \Myth\Auth\Filters\LoginFilter::class,
    'role'       => \Myth\Auth\Filters\RoleFilter::class,
    'permission' => \Myth\Auth\Filters\PermissionFilter::class,`

