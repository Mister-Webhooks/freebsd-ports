PORTNAME=	libconfig
PORTVERSION=	1.7.3
CATEGORIES=	devel
MASTER_SITES=	https://github.com/hyperrealm/${PORTNAME}/releases/download/v${PORTVERSION}/

MAINTAINER=	ntarmos@ceid.upatras.gr
COMMENT=	Simple library for processing structured configuration files
WWW=		https://www.hyperrealm.com/libconfig/libconfig.html

LICENSE=	LGPL21

USES=		libtool pathfix
USE_LDCONFIG=	yes

GNU_CONFIGURE=	yes
CONFLICTS=	wand-libconfig

OPTIONS_DEFINE=	INFO
OPTIONS_DEFAULT=INFO

INFO_INFO=	libconfig
INFO_CONFIGURE_OFF=	--disable-doc
INFO_USES=	makeinfo

.include <bsd.port.mk>
