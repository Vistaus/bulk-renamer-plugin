project(
    'io.github.jeremypw.bulk-renamer-plugin', 'vala', 'c',
    meson_version : '>= 0.46',
    version: '1.0.0'
)

i18n = import('i18n')

add_global_arguments('-DGETTEXT_PACKAGE="io.github.jeremypw.bulk-renamer-plugin"', language:'c')

parent_project_name='io.elementary.files'

core_deps = [
    dependency('glib-2.0'),
    dependency('gobject-2.0'),
    dependency('pantheon-files-core')
]

vala_version_required = '0.40.0'
vala = meson.get_compiler('vala')
posix_dep = vala.find_library('posix')
#meson.add_install_script('meson/post_install.py')

subdir('data')
subdir('src')
subdir ('po')
