PORTNAME=	yuicompressor
PORTVERSION=	2.4.8
PORTREVISION=	3
CATEGORIES=	www java
#MASTER_SITES=	http://tml.github.io/yui/
MASTER_SITES+=	LOCAL/az
EXTRACT_SUFX=	.jar
EXTRACT_ONLY=	# empty

MAINTAINER=	citrin@citrin.ru
COMMENT=	The Yahoo! JavaScript and CSS Compressor
WWW=		https://yui.github.io/yuicompressor/

LICENSE=	BSD3CLAUSE MPL20
LICENSE_COMB=	multi

USES=		java

NO_WRKSUBDIR=	yes

NO_BUILD=	yes
NO_ARCH=	yes

PLIST_FILES=	bin/yuicompressor %%JAVAJARDIR%%/yuicompressor.jar
SUB_FILES=	yuicompressor

do-install:
	${INSTALL_DATA} ${DISTDIR}/${DISTNAME}.jar ${STAGEDIR}${JAVAJARDIR}/yuicompressor.jar
	${INSTALL_SCRIPT} ${WRKDIR}/yuicompressor ${STAGEDIR}${PREFIX}/bin

.include <bsd.port.mk>
